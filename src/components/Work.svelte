<script>
  export let project;
</script>

<div class="work">
  <div class="work__image-container">
    <img src={"images/" + project.image} alt={project.name + " screenshot"} />
  </div>
  <div class="work__description-container">
    <h3 class="work__name">{project.name}</h3>
    <p class="work__description">{project.description}</p>
    <div class="btn-group">
      <div class="btn-in">
        <a href={project.repository} target="_blank" rel="noopener noreferrer">
          <button class="btn btn-primary">Source Code</button>
        </a>
      </div>
      {#if project.liveWebsite}
        <div class="btn-in">
          <a
            href={project.liveWebsite}
            target="_blank"
            rel="noopener noreferrer"
          >
            <button class="btn btn-primary">Live Website</button>
          </a>
        </div>
      {/if}
    </div>
  </div>
</div>

<style>
  .work {
    display: flex;
    flex-direction: column;
    margin-bottom: 5rem;
  }
  .work img {
    width: 18rem;
    height: 18rem;
    object-fit: cover;
  }
  .work__name {
    font-size: 2.5rem;
    margin-bottom: 2rem;
  }
  .work__description {
    font-size: 1.5rem;
    margin-bottom: 2rem;
  }
  @media only screen and (min-width: 1024px) {
    .work {
      flex-direction: row;
    }
    .work__description-container {
      margin-left: 2rem;
      height: 180px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }
    .work .__description {
      font-size: 2rem;
      vertical-align: middle;
    }
  }
</style>
