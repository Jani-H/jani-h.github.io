<script>
  import Carousel from 'svelte-carousel';
  import Button from '../reusable/Button.svelte';
  import { slide } from 'svelte/transition';

  let showInfo = false;
  function toggleInfo() {
    showInfo = !showInfo;
  }
</script>

<main transition:slide>
  <div class="work-box">
    <h2>Tournament Assembly</h2>
    <p class="description">
      I worked on this with a group of students for a JAMK assignment. I created
      necessary components, content and made the site responsive for mobile
      devices.
    </p>
    <a
      href="https://github.com/jamktiko/TournamentAssembly-svelte"
      target="_blank"
    >
      <img id="github" src="./images/GitHub_Logo_White.png" alt="GitHubImage" />
    </a>
    <div>
      <div class="show-info">
        <Button class="info-button" on:cClick={toggleInfo}
          >What I worked on this project in detail</Button
        >
      </div>
      {#if showInfo}
        <div transition:slide>
          <p class="details">
            I worked as frontend developer and scrum master in this project. I
            oversaw creating a responsive mobile design for our application and
            I also created quite a few of the applications frontend components.
            I took my time in creating a solid user experience for different
            mobile devices by creating fluid interface.
          </p>
          <p class="details">
            In terms of component creation, I developed various essential
            components that formed the backbone of our application. Through
            testing and based on user feedback I also created intuitive
            navigation and interactive elements making the application more
            user-friendly.
          </p>
          <p class="details">
            My role also extended beyond design and development; I took charge
            of being our teams Scrum Master. While our scrum meetings maintained
            a relaxed atmosphere, I ensured that the team stayed on track with
            our project timelines. As the Scrum Master I encouraged open
            communication and allowing team members to express ideas and
            concerns freely. By doing this I fostered a positive working
            environment for our team.
          </p>
          <p class="details">
            Despite the informal nature of our scrum meetings, I prioritized the
            adherence to project goals and timelines. Through effective backlog
            management, sprint planning, and regular retrospectives, our team
            successfully navigated the development process. The loose structure
            of our meetings did not compromise the precision and efficiency
            required to complete our project.
          </p>
          <p class="details">
            In summary, working on this school project involved me working in
            different roles which not only included frontend developing and
            working as the teams Scrum Master. The combination of technical
            proficiency, design sensibility and adept project management ensured
            the successful delivery of a cohesive and functional application.
          </p>
        </div>
      {/if}
    </div>
    <Carousel>
      <img
        class="image"
        src="./images/tournament-assembly-main-page.png"
        alt="TournamentAssemblyPicture"
      />
      <img
        class="image"
        src="./images/tournament-assembly-groups.png"
        alt="TournamentAssemblyPicture"
      />
      <img
        class="image"
        src="./images/tournament-assembly-league.png"
        alt="TournamentAssemblyPicture"
      />
      <img
        class="image"
        src="./images/tournament-assembly-playoffs.png"
        alt="TournamentAssemblyPicture"
      />
      <img
        class="image"
        src="./images/tournament-assembly-scoreboard.png"
        alt="TournamentAssemblyPicture"
      />
      <img
        class="image"
        src="./images/tournament-assembly-responsive-1.png"
        alt="TournamentAssemblyPicture"
      />
      <img
        class="image"
        src="./images/tournament-assembly-responsive-2.png"
        alt="TournamentAssemblyPicture"
      />
    </Carousel>
  </div>
  <hr class="divider" />
  <div class="work-box">
    <h2>Cocktail Library</h2>
    <p class="description">Frontend Project I made for a JAMK assignment.</p>
    <a href="https://github.com/Jani-H/cocktail-library-aa4087" target="_blank">
      <img id="github" src="./images/GitHub_Logo_White.png" alt="GitHubImage" />
    </a>
    <p />
    <Carousel>
      <img
        class="image"
        src="./images/cocktail-library-home.png"
        alt="CocktailLibraryPicture"
      />

      <img
        class="image"
        src="./images/cocktail-library-cocktails.png"
        alt="CocktailLibraryPicture"
      />

      <img
        class="image"
        src="./images/cocktail-library-cocktails-open.png"
        alt="CocktailLibraryPicture"
      />
    </Carousel>
  </div>
</main>

<style>
  main {
    justify-content: center;
  }

  h2 {
    text-align: center;
  }

  a {
    display: flex;
    justify-content: center;
    margin-bottom: 0.25em;
  }

  img {
    width: 100px;
    height: auto;
  }

  .work-box {
    margin: 1em 15em;
  }

  .image {
    width: auto;
    height: 400px;
  }

  .show-info {
    display: flex;
    justify-content: center;
  }

  .description {
    text-align: center;
  }

  hr.divider {
    margin: 0em 20%;
    border-top: 3px solid rgba(255, 255, 255, 1);
  }

  .details {
    margin-bottom: 1em;
  }
</style>
