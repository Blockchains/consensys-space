<script>
  import Button from "./Button.svelte";
</script>

<style>
  #welcome-banner__text-container {
    font-weight: 200;
    font-size: 142px;
    line-height: 173px;
  }

  #tile-wrapper {
    border: 1px solid white;
    display: flex;
    margin-top: 5em;
  }

  .tile {
    border: 1px solid white;
    display: flex;
    flex-direction: column;
    width: 460px;
  }

  .image-wrapper {
    border: 1px solid white;
    height: 260px;
    width: 460px;
  }

  .tile h2 {
    font-weight: bold;
    font-size: 32px;
    line-height: 39px;
  }

  .tile p {
    font-size: 24px;
    line-height: 28px;
  }
</style>

<section>
  <div id="welcome-banner__text-container">
    <p>open</p>
    <p>source</p>
    <p>space</p>
  </div>
  <div id="tile-wrapper">
    <div class="tile">
      <div class="image-wrapper">
        <img src="placeholder" alt="planetary resources" />
      </div>
      <h2>Unlocking Planetary Resources’ Intellectual Property</h2>
      <p>A decade of innovation, yours to build upon</p>
      <Button text="more" to="/pr" />
    </div>
    <div class="tile">
      <div class="image-wrapper">
        <img src="placeholder" alt="trusat" />
      </div>

      <h2>Citizen-Powered Space Sustainability</h2>
      <p>
        Designed and incubated by ConsenSys, built and powered by a global open
        source community.
      </p>
      <Button text="more" to="/trusat" />
    </div>
  </div>

</section>
