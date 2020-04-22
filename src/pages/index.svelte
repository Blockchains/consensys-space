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
    font-family: Montserrat;
    font-weight: 200;
    font-size: 142px;
    line-height: 173px;
  }

  #tile-wrapper {
    display: flex;
    flex-wrap: wrap;
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

  @media (min-width: 1200px) and (max-width: 1400px) {
    main {
      margin-top: -650px;
    }
  }

  @media (min-width: 1000px) and (max-width: 1200px) {
    main {
      margin-top: -550px;
    }
  }

  /* Tablet */
  @media (min-width: 600px) and (max-width: 1200px) {
    main {
      padding: 0em 4em 0em 4em;
    }

    #tagline {
      font-weight: 200;
      font-size: 100px;
      line-height: 120px;
    }

    #pr-tile {
      margin-bottom: 6em;
    }

    .tile {
      height: auto;
    }

    .tile p {
      margin-bottom: 1em;
    }
  }

  @media (min-width: 800px) and (max-width: 1000px) {
    main {
      margin-top: -450px;
    }
  }

  @media (min-width: 600px) and (max-width: 800px) {
    main {
      margin-top: -350px;
    }
  }

  /* Mobile  */
  @media (max-width: 600px) {
    main {
      margin-top: -120px;
      padding: 0em 1em 0em 1em;
    }

    #tagline {
      font-weight: 200;
      font-size: 60px;
      line-height: 80px;
    }

    #pr-tile {
      margin-bottom: 6em;
      margin-right: 0;
    }

    .tile {
      height: auto;
      width: 100%;
    }

    .image-wrapper {
      width: 100%;
    }

    .tile p {
      margin-bottom: 1em;
    }
  }
</style>

<WelcomeBanner />
<main>
  <div id="tagline">
    <p>OPEN</p>
    <p>SOURCE</p>
    <p>SPACE</p>
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
