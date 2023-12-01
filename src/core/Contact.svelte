<script>
  import { slide } from 'svelte/transition';
</script>

<main transition:slide>
  <div class="contact-detail">
    <h2>Email</h2>
    <a href="mailto:AA4087@student.jamk.fi"><p>AA4087@student.jamk.fi</p></a>
  </div>
  <div class="contact-detail">
    <h2>LinkedIn</h2>
    <a href="https://www.linkedin.com/in/jani-haakana/" target="_blank">
      <p>https://www.linkedin.com/in/jani-haakana/</p>
    </a>
  </div>
</main>

<style>
  main {
    margin: 1em 4em;
    border-style: solid;
    border-color: black;
    border-width: 1px;
    border-radius: 5px;
    padding: 0.5em 0.5em;
    background-color: rgba(0, 0, 0, 0.5);
  }

  .contact-detail {
    margin: 0.5em;
  }

  h2 {
    text-align: center;
  }

  p {
    font-size: 1.2em;
  }

  a {
    justify-content: center;
    text-align: center;
  }

  @media screen and (max-width: 700px) {
    main {
      margin: 1em 1em;
    }
  }
</style>
