<script>
  import { slide } from 'svelte/transition';
</script>

<main transition:slide>
  <h1>
    Welcome to my portfolio! You can find info about me and projects I have
    worked on from the menu above.
  </h1>
</main>

<style>
  main {
    padding-top: 20vh;
  }

  h1 {
    padding: 1em;
    text-align: center;
  }
</style>
