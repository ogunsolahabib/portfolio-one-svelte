<script>
  let socials = [
    {
      title: "Github",
      url: "https://github.com/ogunsolahabib",
      icon: "fab fa-github",
    },
    {
      title: "LinkedIn",
      url: "https://linkedin.com/in/habib-ogunsola-92b79a15a/",
      icon: "fab fa-linkedin",
    },
    {
      title: "Twitter",
      url: "https://twitter.com/ha_beeeb",
      icon: "fab fa-twitter",
    },
    {
      title: "Instagram",
      url: "https://instagram.com/ha_beeeb_",
      icon: "fab fa-instagram",
    },
  ];
</script>

<footer>
  <p class="site-details">
    Built with <a
      target="_blank"
      rel="noopener noreferrer"
      href="https://svelte.dev">Svelte.js</a
    >
    and hosted on
    <a target="_blank" rel="noopener noreferrer" href="https://netlify.com"
      >Nelify</a
    >
  </p>
  <div class="copyright-and-socials">
    <p class="copyright">&copy; {new Date().getFullYear()} Habib Ogunsola</p>
    <ul class="socials">
      {#each socials as social}
        <li>
          <a
            target="_blank"
            rel="noopener noreferrer"
            href={social.url}
            title={social.title}
          >
            <i class={social.icon} />
          </a>
        </li>
      {/each}
    </ul>
  </div>
</footer>

<style>
  .site-details a {
    text-decoration: underline;
  }
  footer > div.copyright-and-socials {
    display: flex;
    flex-direction: column-reverse;
  }
  footer ul {
    display: flex;
    align-items: center;
  }
  footer .copyright {
    margin-top: 1rem;
  }

  footer ul li {
    color: #fff;
    margin-right: 2rem;
    font-size: 2rem;
  }
  p.site-details {
    margin-bottom: 1rem;
  }
  @media screen and (min-width: 768px) {
    footer div.copyright-and-socials {
      flex-direction: row;
      justify-content: space-between;
      text-align: center;
      align-items: center;
    }
    footer .copyright {
      margin-top: 0;
    }
  }
</style>
