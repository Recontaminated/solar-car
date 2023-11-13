

<header>
            <div class="poly-brand">
                <a href="https://polytechnic.org" id="poly-button">
                    <img src="https://bbk12e1-cdn.myschoolcdn.com/ftpimages/270/logo/masterlogo-white.png" alt="Polytechnic School | Pasadena, CA" id="poly-image">
                </a>
            </div>
            <div class="nav-wrapper">
                <nav>
                    <ul>
                        <!-- <li><a href="/about" class="effect-3">About</a></li> -->


                        <li><a href="/" class="">Home</a></li>
                        <li><a href="/blog" class="">Blog</a></li>
                        <li><a href="/projects" class="">Car</a></li>
                        <li><a href="/sponsors" class="">Sponsors</a></li>
                    </ul>
                </nav>
        </div>
</header>
<script>
    import '$lib/styles/hoverEffects.scss';
    import {page} from "$app/stores";
    import {onMount} from "svelte";
    onMount(()=>{
        //get all links in nav
        let links = document.querySelectorAll('nav a');
        //set active link
        console.log($page)
        links.forEach(link => {

            console.log("active link: " + link.href + " " + $page.url.href)
            if (link.href === $page.url.href) {
                link.classList.add('active');
                // link.classList.remove('effect-3');
            }
        });
    })


</script>


<style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap');
    .brand {
        font-family:Inter, Roboto, sans-serif;
        font-weight: 700;
        color: white;
        padding-bottom: 20px;

    }

    nav {
        /*padding-top: 15px;*/
        font-size: 0.9rem;
        font-family: apple-system,Inter, sans-serif;
        font-weight: 300;
    }

    header {
        /* background: lightskyblue; */
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    /*    turn down opacity to show image behind it*/
        background-color: #161616;

        /*backdrop-filter: blur(10px);*/
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        z-index: 100;
    }
    li {
        background-color: rgba(5,5,5,1);
        border-radius: 5px;
        height: 36px;
        min-width: 64px;
        padding: 0 16px;
        transition: color 0.2s ease-out, background-color 0.2s ease-out;
        }

    li a {
        /*center items vertically*/
        display: flex;
        align-items: center;
        height: 100%;
        color: white;
        justify-content: center;
    }

    li:hover {
        background-color: rgba(100,100,100,1);
    }

    ul {
        margin: 0;
        list-style-type: none;
        display: flex;
        gap: 2rem;
    }

    .nav-wrapper {
        /*font-size: 1.2rem;*/
        font-size: 1.3rem;
        height: 80px;
        margin-right: 5rem;
        display: flex;
        align-items: center;
    }

    a {
        text-decoration: none;
        color: #bbb;

    }

    #poly-button::before {
        content: "";
        width: 6.25rem;
        height: 5rem;
        float: left;
        background-image: url("https://images.duckarmada.com/pgudhlBqKwJf/direct.png");
        background-size: 5rem;
        background-repeat: no-repeat;
        background-position: left center;

    }
    #poly-button {
    /*    put all items inlione and centered vertically*/
        display: flex;
        align-items: center;
        height: 100%;
        padding-right: 1rem;
    }

.poly-brand {
    }



    #poly-image {
        width: 22.5rem;
    }
</style>