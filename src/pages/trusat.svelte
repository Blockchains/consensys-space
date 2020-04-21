<script>
  import Button from "../Button.svelte";
</script>

<style>
  main {
    max-width: 1200px;
    margin: 0 auto;
  }

  section {
    max-width: 600px;
  }

  section:nth-of-type(2) {
    padding-bottom: 6em;
  }

  h1 {
    font-family: Montserrat;
    font-weight: 300;
    font-size: 72px;
    line-height: 88px;
    margin-bottom: 0.25em;
  }

  h2 {
    font-family: Roboto;
    font-weight: bold;
    font-size: 32px;
    line-height: 37px;
    margin-bottom: 1em;
  }

  a {
    color: white;
  }

  #iframe-wrapper {
    height: 0;
    overflow: hidden;
    position: relative;
    padding-bottom: 56.25%;
  }

  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  p {
    font-family: Roboto;
    font-size: 24px;
    line-height: 32px;
    margin-bottom: 1em;
  }

  p:nth-of-type(2) {
    margin-bottom: 2em;
  }
</style>

<main>
  <img src="" alt="pr header" />
  <section>
    <h1>Citizen-Powered Space Sustainability</h1>
    <h2>
      <a href="https://trusat.org" target="_blank" rel="noopener noreferrer">
        TruSat
      </a>
      is an open-source system for creating a globally-accessible, trusted
      record of satellite orbital positions.
    </h2>
  </section>

  <div id="iframe-wrapper">
    <iframe
      className="welcome__iframe"
      title="TruSat explainer video"
      src="https://www.youtube.com/embed/H-J7zngl6xE"
      frameBorder="0"
      allow="accelerometer; autoplay; encrypted-media; gyroscope;
      picture-in-picture"
      allowFullScreen="allowfullscreen"
      mozallowullscreen="mozallowfullscreen"
      msallowfullscreen="msallowfullscreen"
      oallowfullscreen="oallowfullscreen"
      webkitallowfullscreen="webkitallowfullscreen"
      modestbranding="1" />
  </div>

  <section>
    <p>
      TruSat is primarily designed to enable the assessment of satellite
      operations in the context of space sustainability standards.
    </p>
    <p>
      ConsenSys Space incubated the project, releasing an alpha in October 2019,
      before handing control of the project to the community in April 2020.
    </p>
    <Button to="https://trusat.org" text="visit trusat" />
  </section>

</main>
