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
    width: 300px;
  }

  @media (max-width: 600px) {
    a {
      display: none;
    }
  }
</style>

<a href="/">
  <img src={'./images/consensys_space_logo.png'} alt="c space logo" />
</a>
<Router {routes} />
