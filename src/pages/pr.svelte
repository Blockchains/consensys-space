<script>
  const patents = [
    {
      number: "9,796,486",
      origin: "USA",
      date: "October 24, 2017",
      title: "Integrated Propulsion and Primary Structure for Microsatellites"
    },
    {
      number: "9,499,284",
      origin: "USA",
      date: "November 22, 2016",
      title:
        "Dual Use Imaging and Optical Communications System for Microsatellites"
    },
    {
      number: "9,499,284",
      origin: "USA",
      date: "August 9, 2016",
      title:
        "Space-Based Structures and Methods of Delivering Space-Sourced Materials "
    },
    {
      number: "9,499,284",
      origin: "USA",
      date: "February 23, 2016",
      title: "Method, Apparatus, and System for Asteroid Prospecting and Mining"
    },
    {
      number: "D756,284",
      origin: "USA",
      date: "May 24, 2016",
      title: "Spacecraft System"
    }
  ];
</script>

<style>
  main {
    max-width: 1200px;
    margin: 0 auto;
  }

  section {
    border: 1px solid red;
    margin-bottom: 5em;
  }

  h1 {
    font-family: Montserrat;
    font-style: normal;
    font-weight: 300;
    font-size: 64px;
    line-height: 78px;
  }

  .image-copy-wrapper {
    margin: 3em 0em 4em 0em;
    display: flex;
  }

  .image-copy-wrapper img {
    width: 50%;
  }

  .image-copy-wrapper div {
    width: 50%;
  }

  .image-copy-wrapper p:first-of-type {
    font-family: Roboto;
    font-style: italic;
    font-weight: normal;
    font-size: 16px;
    line-height: 24px;
  }

  .image-copy-wrapper p:nth-of-type(2) {
    font-family: Roboto;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 24px;
  }

  #main-copy {
    max-width: 600px;
  }

  #main-copy p {
    font-family: Roboto;
    font-size: 24px;
    line-height: 32px;
    margin-top: 1em;
  }

  #patents-section h2 {
    font-family: Roboto;
    font-style: normal;
    font-weight: bold;
    font-size: 32px;
    line-height: 37px;
  }

  ul {
    border-top: 1px solid rgba(255, 255, 255, 0.5);
    margin-top: 1em;
    margin-bottom: 5em;
  }

  .list-item {
    border-bottom: 1px solid rgba(255, 255, 255, 0.5);
    margin-top: 1em;
    padding-bottom: 1em;
  }

  .list-item p {
    font-family: Roboto;
    font-size: 16px;
    line-height: 32px;
  }

  .list-item a {
    color: white;
    font-family: Roboto;
    font-size: 24px;
    line-height: 32px;
  }

  #disclaimer-copy {
    font-family: Roboto;
    font-size: 16px;
    line-height: 19px;
    max-width: 600px;
  }

  #disclaimer-copy p {
    margin-bottom: 1em;
  }
</style>

<img src="./images/pr_header.jpg" alt="pr header" />
<main>
  <section id="copy-section">
    <h1>Planetary Resources Intellectual Property Pledge</h1>
    <div class="image-copy-wrapper">
      <img src="" alt="launch party" />
      <div>
        <p>
          I frequently get the question: ‘what are you doing with Planetary
          Resources?’ The person asking generally assumes we’re getting into the
          business of harvesting the natural resources of celestial bodies.
          Instead, as you now know, we are working to harness the human
          resources of this celestial body—all the talent, wisdom, and
          creativity on the sidelines—and convert this potential energy into
          progress in space, and here on Earth.
        </p>
        <p>~Joseph Lubin, October 21, 2019</p>
      </div>

    </div>

    <div id="main-copy">
      <p>
        ConsenSys acquired Planetary Resources, a pioneering space company, in
        October of 2018. Over the course of nearly a decade, Planetary Resources
        produced innovations at every step along the path to its bold mission of
        harnessing the natural resources of celestial bodies, from spacecraft
        design to tools for technical and economic analysis of resources
        throughout our solar system. Consonant with ConsenSys’ belief in the
        power of open innovation to solve the toughest challenges, on our planet
        and beyond, we’re making the Planetary Resources intellectual property
        we own available to you to build upon, as follows.
      </p>
      <p>
        ConsenSys irrevocably pledges that it will not initiate a lawsuit
        against any person for infringing a Planetary Resource Patent or Space
        Technology Intellectual Property, as defined below.
      </p>
      <p>
        “Planetary Resource Patent” means the following patents acquired by
        ConsenSys from Planetary Resources
      </p>
    </div>
  </section>

  <section id="patents-section">
    <h2>Patents</h2>
    <ul>
      {#each patents as patent (patent.date)}
        <li class="list-item">
          <p>
            {`Patent No ${patent.number} | ${patent.origin} | ${patent.date}`}
          </p>
          <a href="/placeholder" target="_blank" rel="noopener noreferrer">
            {patent.title}
          </a>
        </li>
      {/each}
    </ul>

    <div id="disclaimer-copy">
      <p>
        "Space Technology Intellectual Property” means all unregistered
        intellectual property in space exploration technology, including Trade
        Secrets, acquired by ConsenSys from Planetary Resources.
      </p>
      <p>
        This Intellectual Property Pledge does not encompass Trademark rights.
      </p>
      <p>
        ConsenSys will endeavor to make previously unpublished Planetary
        Resources materials available, to the extent permitted by export
        controls and other applicable laws.
      </p>
    </div>
  </section>

</main>
