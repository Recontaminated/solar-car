<script>
    import { onMount,tick } from 'svelte';
    let visible = false;

    onMount(async () => {
        // await tick();
        visible = true;
    });
</script>

<div class="fade-in" class:visible>

    <slot></slot>
</div>

<style>
    .fade-in{
        opacity: 0;
        transform: translateY(100px);
        transition: opacity 0.3s ease, transform 0.6s ease;
    }

    .fade-in.visible {
        opacity: 1;
        transform: translateY(0);
    }
</style>
