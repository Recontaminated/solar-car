<script>
    import Header from "$lib/components/Header.svelte";
    import FadeIn from "$lib/components/FadeIn.svelte";
</script>

<div class="main">
    <Header></Header>
    <div class="main-section">
        <FadeIn>
        <div class="hero">
            <h1>POLY ENGINEERING</h1>
        </div>
            <div id="learn-more">
                <a href="#learn-more">Learn More</a>
            </div>

        </FadeIn>

    </div>

</div>
<FadeIn>
<div class="scroll">
    <img src="/assets/down-arrow.png">
</div>
</FadeIn>
<div class="introduction">
    <div class="info-section">

        <h1 id="info-title">DRIVEN BY INNOVATION</h1>
        <p id="info-text"> Founded in 2020. The Poly Engineering Club is student run, fueled by its passion for creating sustainable energy solutions. We provide unique opportunities for students to engage with hands-on engineering while striving towards a more sustainable future. Last year, we raced in the Texas Solar Car Challenge and placed 2nd in the classic division. This year, we hope to use our past learnings and apply them as we build a new car to race in the advanced division. </p>

    </div>

</div>
<!--<div class="competition">-->
<!--    <div class="comp-info">-->

<!--        <h1 id="comp-title">Texas Solar Car Challenge</h1>-->
<!--        <p id="comp-text"> Founded in 2020. The Poly Engineering Club is student run, fueled by its passion for creating sustainable energy solutions. We provide unique opportunities for students to engage with hands-on engineering while striving towards a more sustainable future. Last year, we raced in the Texas Solar Car Challenge and placed 2nd in the classic division. This year, we hope to use our past learnings and apply them as we build a new car to race in the advanced division. </p>-->
<!--        <img id = "texas_img" src="https://cdn.discordapp.com/attachments/1149899922838130809/1175568975661379594/fortworth.png?ex=656bb4ec&is=65593fec&hm=d9440b0e3d70627f942fd1473064ca2257fc04ef93249a9255694e01632cf117&">-->
<!--    </div>-->

<!--</div>-->


<style lang="scss">
  @font-face {
    font-family: "neuron";
    src: url("/fonts/Exo2-Regular.ttf");
  }
  .main {
    height: 100vh;
    //-webkit-background-size: cover;
    //background-size: cover;
    background-image: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url("https://images.duckarmada.com/dR2VFyjlFtMm/direct.png");
    //move the background image left

    background-size: cover  ;
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
    text-align: center;
    padding: 0;

  }

  .buttons a {
    margin: 0 10px;
    padding: 7px 15px;
    background-color: var(--organizationgray);
    border-radius: 5px;
    text-align:center;
    //width: 100%;
  }
  li a {
    width: 100%;
    background-color: red;
  }

  .buttons a:hover {
    background-color: var(--accentcolor);
  }

  .hero {
    font-weight: 500;
    font-size: 70px;
    font-family: neuron;
    letter-spacing: 8px;
  //  center
    text-align: center;
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

  #info-title{
    font-size: 40px;
  }
  .info-section{
    margin-top: 100px;
    text-align: center;
    margin-left: 400px;
    margin-right: 400px;
    margin-bottom: 100px;
  }
  #info-text{
    margin-top: 20px;
    line-height: 2;
  }

  .competition{
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }

  #comp-title{
    font-size: 40px;
  }
  .comp-info{
    margin-top: 100px;
    text-align: center;
    margin-left: 400px;
    margin-right: 400px;
    margin-bottom: 100px;
    width: 50%;
  }
  #comp-text{
    margin-top: 20px;
    line-height: 2;
    width: 50%;
  }
  #texas_img{
    width: 50%;
  }

  #learn-more {
  width: 120px;
    margin-top: 100px;
  //  center the div
    margin-left: auto;
    margin-right: auto;
    background-color: #f28b00;
    border-radius: 5px;
    height: 40px;
    display: flex;
    align-items: center;
    justify-content: center;

  }
  .scroll {
    filter: brightness(0) invert(1) opacity(0.7);
    bottom: 5vh;
    position: absolute;
  //  center it
    left: 50%;
    transform: translateX(-50%);
  }
  html{
    scroll-behavior: smooth;
  }
  .scroll img {
    height: 60px;
  }

</style>