<script>
  const patents = [
    {
      number: "9,796,486",
      origin: "USA",
      date: "October 24, 2017",
      title: "Integrated Propulsion and Primary Structure for Microsatellites",
      link: "https://patents.google.com/patent/US9796486B1/en"
    },
    {
      number: "9,499,284B1",
      origin: "USA",
      date: "November 22, 2016",
      title:
        "Dual Use Imaging and Optical Communications System for Microsatellites",
      link: "https://patents.google.com/patent/US9499284B1/en"
    },
    {
      number: "9,409,658",
      origin: "USA",
      date: "August 9, 2016",
      title:
        "Space-Based Structures and Methods of Delivering Space-Sourced Materials",
      link: "https://patents.google.com/patent/US9409658B1/"
    },
    {
      number: "9,266,627B1",
      origin: "USA",
      date: "February 23, 2016",
      title:
        "Method, Apparatus, and System for Asteroid Prospecting and Mining",
      link: "https://patents.google.com/patent/US9266627B1/en"
    },
    {
      number: "D756,284",
      origin: "USA",
      date: "May 24, 2016",
      title: "Spacecraft System",
      link: "https://patents.google.com/patent/USD756886S1/"
    }
  ];
</script>

<style>
  #hero-container {
    position: relative;
    height: 400px;
    overflow: auto;
    z-index: -1;
    width: 100%;
    -webkit-mask-image: linear-gradient(to bottom, black 50%, transparent 100%);
    mask-image: linear-gradient(to bottom, black 50%, transparent 100%);
  }

  #hero-container::-webkit-scrollbar {
    display: none;
  }

  #hero-container img {
    height: auto;
    /* Pulls image up */
    margin-top: -250px;
    width: 100%;
  }

  main {
    max-width: 1200px;
    margin: 0 auto;
    margin-bottom: 10em;
    margin-top: -5em;
  }

  section {
    margin-bottom: 5em;
  }

  h1 {
    font-family: Montserrat;
    font-weight: 300;
    font-size: 64px;
    line-height: 78px;
  }

  .image-copy-wrapper {
    margin: 3em 0em 4em 0em;
    display: flex;
  }

  .image-copy-wrapper div {
    width: 50%;
  }

  .image-wrapper {
    margin-right: 2em;
  }

  .image-wrapper img {
    width: 100%;
  }

  .image-copy-wrapper p:first-of-type {
    font-family: Roboto;
    font-style: italic;
    font-weight: normal;
    font-size: 16px;
    line-height: 24px;
    margin-bottom: 1em;
  }

  .image-copy-wrapper p:nth-of-type(2) {
    font-family: Roboto;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 24px;
  }

  #main-copy {
    max-width: 800px;
  }

  #main-copy p {
    font-family: Roboto;
    font-size: 24px;
    line-height: 32px;
    margin-top: 1em;
  }

  /* The last block of text styled to match the disclaimer */
  #main-copy p:nth-of-type(3) {
    font-size: 18px;
    line-height: 24px;
  }

  #main-copy p:nth-of-type(4) {
    font-size: 18px;
    line-height: 24px;
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
    font-size: 18px;
    line-height: 24px;
    max-width: 800px;
  }

  #disclaimer-copy p {
    margin-bottom: 1em;
  }

  /* Tablet */
  @media (min-width: 600px) and (max-width: 1200px) {
    main {
      padding: 0em 4em 0em 4em;
    }

    #hero-container img {
      /* Pulls image up */
      margin-top: -120px;
    }
  }

  /* Mobile */
  @media (max-width: 600px) {
    main {
      padding: 0em 1em 0em 1em;
      margin-top: 0;
    }

    #hero-container {
      height: 200px;
    }

    #hero-container img {
      /* Pulls image up */
      margin-top: 0px;
    }

    h1 {
      font-weight: 300;
      font-size: 40px;
      line-height: 45px;
    }

    .image-copy-wrapper {
      flex-wrap: wrap;
    }

    .image-copy-wrapper div {
      width: 100%;
    }

    .image-wrapper {
      margin-bottom: 1em;
      margin-right: 0;
    }

    #main-copy p {
      font-family: Roboto;
      font-size: 18px;
      line-height: 24px;
      margin-top: 1em;
    }

    #main-copy p:nth-of-type(3) {
      font-size: 14px;
      line-height: 18px;
    }

    #main-copy p:nth-of-type(4) {
      font-size: 14px;
      line-height: 18px;
    }

    .list-item p {
      font-size: 20px;
      line-height: 24px;
    }

    .list-item a {
      color: white;
      font-family: Roboto;
      font-size: 16px;
      line-height: 24px;
      /* Highlight that its a link on mobile */
      text-decoration: underline;
    }

    #disclaimer-copy {
      font-size: 14px;
      line-height: 18px;
    }
  }
</style>

<div id="hero-container">
  <img
    src="https://consensys-space-assets.s3.amazonaws.com/pri_hero.jpg"
    alt="pr header" />
</div>

<main>
  <section id="copy-section">
    <h1>Planetary Resources Intellectual Property Pledge</h1>
    <div class="image-copy-wrapper">
      <div class="image-wrapper">
        <img
          src="https://consensys-space-assets.s3.amazonaws.com/trusat_launch.jpg"
          alt="launch party" />
      </div>
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
        against any party for infringing a Planetary Resources Patent or
        Planetary Resources Intellectual Property, for so long as such party is
        acting in good faith. The key terms of this pledge are defined below.
      </p>
      <p>
        A party is "acting in good faith" for so long as such party and its
        related or affiliated companies have not filed a lawsuit or other legal
        proceeding for patent or intellectual property infringement, or obtained
        a direct financial interest in such lawsuit or other legal proceeding,
        against ConsenSys or any entity controlled by ConsenSys or against any
        third party based in whole or in part on any product or service
        developed by or on behalf of ConsenSys or any entity controlled by
        ConsenSys.
      </p>
      <p>
        “Planetary Resources Patent” means the following patents acquired by
        ConsenSys from Planetary Resources:
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
          <a href={patent.link} target="_blank" rel="noopener noreferrer">
            {patent.title}
          </a>
        </li>
      {/each}
    </ul>

    <div id="disclaimer-copy">
      <p>
        "Planetary Resources Intellectual Property” means all unregistered
        intellectual property in space exploration technology, including trade
        secrets, to the extent acquired by ConsenSys from Planetary Resources.
      </p>
      <p>
        This intellectual property pledge does not encompass any trademark
        rights.
      </p>
    </div>
  </section>
</main>
