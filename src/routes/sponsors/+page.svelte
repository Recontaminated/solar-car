<script>
    import Header from "$lib/components/Header.svelte";
</script>
<div class="main">
<div class="header-cont">
    <Header></Header>
</div>

<div class="main-cont">
    <div class="heading">
        <h1><b>Sponsors</b></h1>
        <h4>Interested in becoming a sponsor? Click <u>here</u></h4>
    </div>

    <div class="logos">
        <div class="tier1">
            <h3>Platinum Support</h3>
            <div class="company">
                <div class="logo">
                    <!--            logo goes in this div-->
                    <img src="https://images.duckarmada.com/LtJ2xWhuJqA6/direct.png">
                </div>
                <div class="description">
                    <!--            company name goes here-->
                    <span>East West Bank is a full-service commercial bank that provides a wide array of services such as retail banking, commercial lending, treasury, residential lending, loans for commercial, construction, and residential real estate projects, and the financing of international trade. </span>
                </div>
            </div>
            <h3>Silver Support</h3>
            <div class="company">
                <div class="logo">
                    <!--            logo goes in this div-->
                    <img src="https://images.duckarmada.com/IHJlh2ebmAcU/direct.png">
                </div>
                <div class="description">
                    <!--            company name goes here-->
                    <span>East West Bank is a full-service commercial bank that provides a wide array of services such as retail banking, commercial lending, treasury, residential lending, loans for commercial, construction, and residential real estate projects, and the financing of international trade. </span>
                </div>
            </div>
            <div class="company">
                <div class="logo">
                    <!--            logo goes in this div-->
                    <img src="https://images.duckarmada.com/YTRO4bdQ0p8X/direct.png">
                </div>
                <div class="description">
                    <!--            company name goes here-->
                    <span>East West Bank is a full-service commercial bank that provides a wide array of services such as retail banking, commercial lending, treasury, residential lending, loans for commercial, construction, and residential real estate projects, and the financing of international trade. </span>
                </div>
            </div>

            <div class="company">
                <div class="logo">
                    <!--            logo goes in this div-->
                    <img src="https://images.duckarmada.com/31zBPlPfBtMh/direct.png">
                </div>
                <div class="description">
                    <!--            company name goes here-->
                    <span>East West Bank is a full-service commercial bank that provides a wide array of services such as retail banking, commercial lending, treasury, residential lending, loans for commercial, construction, and residential real estate projects, and the financing of international trade. </span>
                </div>
            </div>
        </div>

    </div>

</div>
</div>
<style>
    .main{
        background-color:#f6f6f6;
        height: 100%;
        width: 100%;
        color: black;
    }
    .header-cont header {
        position: inherit !important;
    }
    .main-cont{
        padding-top: 90px;
    }
    h1 {
        line-height: 34px;
        height: 40px;
        font-size: 40px;
    }
    .logos{
        width: 100%;

    }
    .company{
        width:80%;
        max-width: 1100px;
        text-align: center;

        margin:auto;
    /*    position elements inline*/
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        height: 15.5rem ;
        margin-bottom:20px;

    }
    .logo  {
        width: 50%;
    }
    .logo-plat img{
        width: 100%;
        height: 100%;
        object-fit: contain;

    }
    .description{
    /*   make it inline with */
        width: 50%;
        text-align:center;

    /*    vertically align*/
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding-left: 20px;

    }
    span {
        display: inline-block;
    }
    h3{
        text-align: center;
        font-size:30px;
        background-color: #bbbbbb;
        margin-bottom: 20px;
    }
    h1{
        text-align:center;
    }
    h4{
        text-align:center;
    }



</style>