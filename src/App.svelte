<script>
  import { Route } from "tinro";
  import Welcome from "./Welcome.svelte";
  import Pr from "./Pr.svelte";
  import Trusat from "./Trusat.svelte";
</script>

<style>
  main {
    max-width: 1200px;
    margin: 0 auto;
  }
</style>

<header>
  <img src="./images/header_logo.jpg" alt="c-space logo" />
</header>

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
