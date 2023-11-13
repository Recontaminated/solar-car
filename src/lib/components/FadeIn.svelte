<script>
    import {afterUpdate, onMount, tick} from 'svelte';
    let visible = false;
    let delay = 3;
    afterUpdate(async () => {
        await tick();
        visible = true;
    });

    onMount(async () => {
        window.addEventListener('scroll', () => {
            const el = document.querySelector('.fade-in');
            const rect = el.getBoundingClientRect();
            const viewHeight = Math.max(document.documentElement.clientHeight, window.innerHeight);
            if (!(rect.bottom < 0 || rect.top - viewHeight >= 0)) {
                visible = true;
            } else {
                visible = false;
            }
        });
    });

</script>

<div class="fade-in" class:visible>

    <slot></slot>
</div>

<style lang="scss">
    .fade-in{
        opacity: 0;
        transform: translateY(100px);
        /*transition: opacity 0.3s ease, transform 0.6s ease;*/
    /*    wait 3 seconds before starting*/
        transition: opacity 0.3s ease 0.5s, transform 0.6s ease 0.5s;
    }

    .fade-in.visible {
        opacity: 1;
        transform: translateY(0);
    }
</style>
