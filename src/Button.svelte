<script>
  export let text;
  export let to;
</script>

<style>
  a {
    align-self: flex-start;
    background: white;
    border-radius: 5px;
    color: black;
    font-weight: bold;
    font-size: 18px;
    line-height: 21px;
    text-align: center;
    letter-spacing: 0.04em;
    padding: 0.5em 1em;
    text-transform: uppercase;
  }
</style>

<a href={to}>{text}</a>
