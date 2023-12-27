<script>
  import "../app.scss";
  import "$lib/styles/style.scss";
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
</svelte:head>

<slot />
<style>

  :root{
    /*--content-width: 1200px;*/
    --content-width: 1160px;
    --font-family-base: "Inter", -sans-serif;
    --font-family-monospace: "Inter", monospace;
    --font-family-heading: "Inter", -sans-serif;
    --font-family-nav: "apple-system", sans-serif;
    --background-color: #181818;
    --gray1: #e6e6e6;
    --fontColorBase: var(--gray1);
    --organizationGray: #2c2c2c;
    --accentColor: #6083ff;
    --bgColor: #181818;
  }

</style>