<script>
  import LottieAnimation from "./LottieAnimation.svelte";
  import Work from "./Work.svelte";

  let projects = [
    {
      name: "Tunez",
      image: "Tunez.png",
      description:
        "Frontend App to search songs, artists and albums from the iTunes API. I used TypeScript, React, Express, Jest.",
      repository: "https://github.com/ogunsolahabib/tunez",
    },
    {
      name: "REST Countries",
      image: "REST_COUNTRIES.png",
      description:
        "The web app shows information of 250 countries and has a light theme and dark theme. I built it using ReactJS and Semantic UI",
      repository: "https://github.com/ogunsolahabib/world-countries",
      liveWebsite: "https://ogunsolahabib.github.io/world-countries",
    },
  ];
  let socials = [
    {
      name: "Linkedin",
      icon: "fab fa-linkedin",
      link: "https://linkedin.com/in/habib-ogunsola-92b79a15a/",
    },
    {
      name: "Github",
      icon: "fab fa-github",
      link: "https://github.com/ogunsolahabib/",
    },

    {
      name: "Twitter",
      icon: "fab fa-twitter",
      link: "https://twitter.com/ha_beeeb",
    },
    {
      name: "Codepen",
      icon: "fab fa-codepen",
      link: "https://codepen.io/ogunsolahabib",
    },
  ];
</script>

<main class="me">
  <section class="section section--hero">
    <div class="hero__about">
      <h1 class="greeting">
        <span class="greeting__hi">Hi, I'm</span> HABIB OGUNSOLA
      </h1>
      <div class="description">
        <p>
          A creative Frontend Engineer and UX enthusiast based in Lagos, Nigeria
          with{" "}
          {new Date().getMonth() > 3 ? "over" : "about"}{" "}
          {new Date().getFullYear() - 2019} years experience in building aesthetically
          pleasing large scale web applications.
        </p>
        <p>Interested in Tech, Business, Combat sports, and Football.</p>
        <br />
        <p>
          I am currently building User Interfaces with awesome people at{" "}
          <a target="_blank" rel="noreferrer" href="https://www.ebanqo.com/">
            eBanqo Inc.
          </a>
        </p>
      </div>
    </div>
    <div class="hero__image">
      <LottieAnimation />
    </div>
  </section>
  <section class="section bottom">
    <div id="contact">
      <h3>Profiles/Contact</h3>
      <div>
        <ul class="set social">
          {#each socials as social}
            <li key={social.name}>
              <a target="_blank" rel="noopener noreferrer" href={social.link}>
                <i class={social.icon} /> <span>{social.name}</span>
              </a>
            </li>
          {/each}
        </ul>
        <div class="v-line" />
        <ul class="set address">
          <li>
            <a href="tel:+2348182141620">
              <i class="fas fa-phone" />
              &nbsp;+2348182141620
            </a>
          </li>
          <li>
            <a href="mailto:ogunsolahabib@yahoo.com">
              <i class="far fa-envelope" />
              &nbsp;
              <span>ogunsolahabib@yahoo.com</span>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </section>

  <h3>Projects</h3>

  {#each projects as project}
    <div>
      <Work {project} />
    </div>
  {/each}
</main>
