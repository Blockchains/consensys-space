<script>
  import { Router } from "@sveltech/routify";
  import { routes } from "@sveltech/routify/tmp/routes";
  import { onMount } from "svelte";
  import { fade } from "svelte/transition";

  let visible = true;

  // hides the c-space logo when user scrolls
  window.addEventListener("scroll", function(event) {
    var scroll = this.scrollY;
    console.log(scroll);

    if (scroll > 40) {
      visible = false;
    } else if (scroll < 40) {
      visible = true;
    }
  });
</script>

<style>
  a {
    color: white;
    left: 1em;
    position: fixed;
    top: 1em;
    width: 300px;
  }
</style>

{#if visible}
  <a transition:fade={{ duration: 500 }} href="/">
    <img
      src={'https://consensys-space-assets.s3.amazonaws.com/consensys_space_logo.png'}
      alt="c space logo" />
  </a>
{/if}

<Router {routes} />
