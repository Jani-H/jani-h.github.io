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
    <div class="work-info">
      <h2>Tournament Assembly</h2>
      <p class="description">
        I worked on this with a group of students in JAMK during our third years
        fall semester.
        <br />
        I worked on the applications frontend and UI/UX where I created necessary
        components, content and made the site responsive for mobile devices.
        <br />
        We used svelte for building the frontend with reactive components, transitions,
        carousels for displaying images. The application also employs responsive
        design through media queries to ensure mobile compatibility.
      </p>
    </div>
    <div class="work-links">
      <a
        href="https://github.com/jamktiko/TournamentAssembly-svelte"
        target="_blank"
      >
        <img
          id="github"
          src="./images/GitHub_Logo_White.png"
          alt="GitHubImage"
        />
      </a>
    </div>
    <div>
      <div class="show-info">
        <Button class="info-button" on:cClick={toggleInfo}
          >What I worked on this project in detail
          {#if !showInfo}
            <svg
              class="expand-arrow"
              xmlns="http://www.w3.org/2000/svg"
              height="24"
              viewBox="0 -960 960 960"
              width="24"
              ><path
                d="M480-345 240-585l56-56 184 184 184-184 56 56-240 240Z"
              /></svg
            >
          {:else}
            <svg
              class="less-arrow"
              xmlns="http://www.w3.org/2000/svg"
              height="24"
              viewBox="0 -960 960 960"
              width="24"
              ><path
                d="m296-345-56-56 240-240 240 240-56 56-184-184-184 184Z"
              /></svg
            >
          {/if}</Button
        >
      </div>
      {#if showInfo}
        <div class="details-whole" transition:slide>
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
    <Carousel
      let:showPrevPage
      let:showNextPage
      autoplay
      autoplayDuration={5000}
      pauseOnFocus
    >
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        slot="prev"
        on:click={showPrevPage}
        class="custom-arrow custom-arrow-prev"
      >
        <svg
          class="back-arrow"
          xmlns="http://www.w3.org/2000/svg"
          height="24"
          viewBox="0 -960 960 960"
          width="24"
          ><path
            d="m242-200 200-280-200-280h98l200 280-200 280h-98Zm238 0 200-280-200-280h98l200 280-200 280h-98Z"
          /></svg
        >
      </div>
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
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        slot="next"
        on:click={showNextPage}
        class="custom-arrow custom-arrow-next"
      >
        <svg
          class="next-arrow"
          xmlns="http://www.w3.org/2000/svg"
          height="24"
          viewBox="0 -960 960 960"
          width="24"
          ><path
            d="m242-200 200-280-200-280h98l200 280-200 280h-98Zm238 0 200-280-200-280h98l200 280-200 280h-98Z"
          /></svg
        >
      </div>
    </Carousel>
  </div>
  <hr class="divider" />
  <div class="work-box">
    <div class="work-info">
      <h2>Cocktail Library</h2>
      <p class="description">
        I created this application as a final assignment for JAMK's Frontend
        Basics course. I had fun creating this application by using an public
        API.
      </p>
    </div>
    <div class="work-links">
      <a
        href="https://github.com/Jani-H/cocktail-library-aa4087"
        target="_blank"
      >
        <img
          id="github"
          src="./images/GitHub_Logo_White.png"
          alt="GitHubImage"
        />
      </a>
    </div>
    <Carousel
      let:showPrevPage
      let:showNextPage
      autoplay
      autoplayDuration={5000}
      pauseOnFocus
    >
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        slot="prev"
        on:click={showPrevPage}
        class="custom-arrow custom-arrow-prev"
      >
        <svg
          class="back-arrow"
          xmlns="http://www.w3.org/2000/svg"
          height="24"
          viewBox="0 -960 960 960"
          width="24"
          ><path
            d="m242-200 200-280-200-280h98l200 280-200 280h-98Zm238 0 200-280-200-280h98l200 280-200 280h-98Z"
          /></svg
        >
      </div>
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
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        slot="next"
        on:click={showNextPage}
        class="custom-arrow custom-arrow-next"
      >
        <svg
          class="next-arrow"
          xmlns="http://www.w3.org/2000/svg"
          height="24"
          viewBox="0 -960 960 960"
          width="24"
          ><path
            d="m242-200 200-280-200-280h98l200 280-200 280h-98Zm238 0 200-280-200-280h98l200 280-200 280h-98Z"
          /></svg
        >
      </div>
    </Carousel>
  </div>
  <hr class="divider" />
  <div class="work-box">
    <div class="work-info">
      <h2>Smart Home Application Design</h2>
      <p class="description">
        I created this at Web UI 2 course in JAMK, it was for the last
        assignment of the course which was to design application from scratch.
        <br />
        I decided to go with Smart Home application. I designed a wireframe and UI-plan
        for the application.
      </p>
    </div>
    <div class="work-links">
      <a
        href="https://www.figma.com/file/ddiSMnFX98X71chtMVBeZt/Lopputy%C3%B6-Rautalankamalli-ja-UI-suunnitelma?node-id=0%3A1"
        target="_blank"
      >
        <img id="figma" src="./images/figma-logo.webp" alt="FigmaImage" />
      </a>
    </div>
    <Carousel
      let:showPrevPage
      let:showNextPage
      autoplay
      autoplayDuration={5000}
      pauseOnFocus
    >
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        slot="prev"
        on:click={showPrevPage}
        class="custom-arrow custom-arrow-prev"
      >
        <svg
          class="back-arrow"
          xmlns="http://www.w3.org/2000/svg"
          height="24"
          viewBox="0 -960 960 960"
          width="24"
          ><path
            d="m242-200 200-280-200-280h98l200 280-200 280h-98Zm238 0 200-280-200-280h98l200 280-200 280h-98Z"
          /></svg
        >
      </div>
      <img class="image" src="./images/ui-final.png" alt="UI-Design1" />
      <img class="image" src="./images/wireframe.png" alt="UI-Design2" />
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        slot="next"
        on:click={showNextPage}
        class="custom-arrow custom-arrow-next"
      >
        <svg
          class="next-arrow"
          xmlns="http://www.w3.org/2000/svg"
          height="24"
          viewBox="0 -960 960 960"
          width="24"
          ><path
            d="m242-200 200-280-200-280h98l200 280-200 280h-98Zm238 0 200-280-200-280h98l200 280-200 280h-98Z"
          /></svg
        >
      </div>
    </Carousel>
  </div>
</main>

<style>
  main {
    justify-content: center;
  }

  h2 {
    text-align: center;
    text-decoration: underline;
  }

  p {
    font-size: 1.2em;
  }

  a {
    display: flex;
    justify-content: center;
    margin-bottom: 0.25em;
    width: 5em;
  }

  img {
    width: 100px;
    height: auto;
  }

  #figma {
    width: 4em;
    height: 4em;
  }

  .work-box {
    margin: 1em 5em;
    border-style: solid;
    border-color: black;
    border-width: 1px;
    border-radius: 5px;
    flex: 1;
    padding: 0.5em 0.5em;
    background-color: rgba(0, 0, 0, 0.5);
  }

  .work-info {
    justify-content: center;
  }

  .work-links {
    display: flex;
    justify-content: center;
    margin: 0.25em 0em;
  }

  .image {
    width: auto;
    height: 400px;
    object-fit: contain;
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

  .details-whole {
    margin-left: 12.5%;
    width: 75%;
  }

  .back-arrow {
    fill: #fff;
    transform: rotate(180deg);
  }

  .next-arrow {
    fill: #fff;
  }

  .expand-arrow {
    fill: #fff;
    position: relative;
    top: 0.5em;
  }

  .less-arrow {
    fill: #fff;
    position: relative;
    top: 0.4em;
  }

  .custom-arrow {
    cursor: pointer;
    width: 40px;
    height: 40px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: rgba(255, 255, 255, 0.25);
    border-radius: 50%;
    position: fixed;
    top: 45%;
    z-index: 10;
  }

  .custom-arrow-prev {
    position: relative;
    margin-right: 0.5em;
    left: 0em;
    top: 11em;
  }

  .custom-arrow-next {
    position: relative;
    margin-left: 0.5em;
    right: 0em;
    top: 11em;
  }

  @media screen and (max-width: 700px) {
    .work-box {
      margin: 1em 1em;
    }
  }

  @media screen and (max-width: 425px) {
    .image {
      width: auto;
      height: 200px;
      object-fit: contain;
    }

    .custom-arrow-prev {
      top: 5em;
    }

    .custom-arrow-next {
      top: 5em;
    }
  }
</style>
