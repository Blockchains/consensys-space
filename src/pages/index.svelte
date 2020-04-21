<script>
  import WelcomeBanner from "../WelcomeBanner.svelte";
  import Button from "../Button.svelte";
</script>

<style>
  main {
    margin: 0 auto;
    max-width: 1200px;
    margin-bottom: 10em;
    margin-top: -725px;
  }

  #tagline {
    font-weight: 200;
    font-size: 142px;
    line-height: 173px;
  }

  #tile-wrapper {
    display: flex;
    margin-top: 6em;
  }

  .tile {
    display: flex;
    flex-direction: column;
    height: 550px;
    width: 460px;
  }

  #pr-tile {
    margin-right: 4em;
  }

  .image-wrapper {
    margin-bottom: 1em;
    width: 460px;
  }

  .tile h2 {
    font-weight: bold;
    font-size: 32px;
    line-height: 39px;
    margin-bottom: 0.5em;
  }

  .tile p {
    font-size: 24px;
    line-height: 28px;
    margin-bottom: auto;
  }
</style>

<WelcomeBanner />
<main>
  <div id="tagline">
    <p>open</p>
    <p>source</p>
    <p>space</p>
  </div>
  <div id="tile-wrapper">
    <div id="pr-tile" class="tile">
      <div class="image-wrapper">
        <img src="./images/asteroids.jpg" alt="planetary resources" />
      </div>
      <h2>Unlocking Planetary Resources’ Intellectual Property</h2>
      <p>A decade of innovation, yours to build upon</p>
      <Button text="more" to="/pr" />
    </div>
    <div class="tile">
      <div class="image-wrapper">
        <img src="./images/asteroids.jpg" alt="trusat" />
      </div>

      <h2>Citizen-Powered Space Sustainability</h2>
      <p>
        Designed and incubated by ConsenSys, built and powered by a global open
        source community.
      </p>
      <Button text="more" to="/trusat" />
    </div>
  </div>
</main>
