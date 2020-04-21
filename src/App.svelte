<script>
  import { Router } from "@sveltech/routify";
  import { routes } from "@sveltech/routify/tmp/routes";
</script>

<style>
  a {
    color: white;
    left: 1em;
    position: fixed;
    top: 1em;
  }
</style>

<a href="/">CONSENSYS SPACE</a>
<Router {routes} />
