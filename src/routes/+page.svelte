<script>
    import Header from "$lib/components/Header.svelte";
    import FadeIn from "$lib/components/FadeIn.svelte";
</script>

<div class="main">
    <Header></Header>
    <div class="main-section">
<!--        <FadeIn>-->
<!--        <div class="hero">-->
            <h1> POLY ENGINEERING CLUB</h1>
<!--        </div>-->
<!--        </FadeIn>-->

    </div>

</div>


<style lang="scss">
  .main {
    height: calc(100vh + 100px);
    //-webkit-background-size: cover;
    //background-size: cover;
    background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 1)), url("https://images.duckarmada.com/rXRXS0YOwv1P/direct.png");
    //background-repeat: no-repeat;
    background-size: cover;
    background-position: center center;
    background-color: var(--background-color)
  }

  .main-section {
    padding-top:30vh;
    height: 100%;
    color: white;


  }

  .buttons {

    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    width: 50%;
    margin-top: 40px;


  }

  .buttons a {
    margin: 0 10px;
    padding: 7px 15px;
    background-color: var(--organizationgray);
    border-radius: 5px;
  }

  .buttons a:hover {
    background-color: var(--accentcolor);
  }

  .hero {
    font-weight: 500;
    font-size: 3rem;
    margin-left: 20px;
  }


  h1 {
    line-height: 34px;
    height: 40px;
  }
  .fancy {
    background-color: rgb(255, 178, 62);
    background-image: linear-gradient(268.67deg, rgb(255, 255, 255) 3.43%, rgb(255, 240, 102) 15.69%, rgb(255, 163, 26) 55.54%, rgb(255, 0, 115) 99%); //https://css-for-js.dev/
    background-size: 100%;
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }
</style>