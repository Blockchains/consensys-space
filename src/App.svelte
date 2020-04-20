<script>
  import { Route } from "tinro";
  import WelcomeBanner from "./WelcomeBanner.svelte";
  import Welcome from "./Welcome.svelte";
  import Pr from "./Pr.svelte";
  import Trusat from "./Trusat.svelte";
</script>

<style>
  header {
    position: fixed;
    left: 20px;
    top: 20px;
  }

  main {
    max-width: 1200px;
    margin: 0 auto;
  }
</style>

<header>
  <img src="./images/header_logo.jpg" alt="c-space logo" />
</header>

<WelcomeBanner />

<main>
  <Route path="/">
    <Welcome />
  </Route>
  <Route path="/pr">
    <Pr />
  </Route>
  <Route path="/trusat">
    <Trusat />
  </Route>
</main>
