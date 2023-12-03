<script>
  import { slide } from 'svelte/transition';
</script>

<main transition:slide>
  <h1>Welcome to my portfolio!</h1>
  <p>
    You can find info about me and projects I have worked on from the menu
    above.
  </p>
</main>

<style>
  main {
    text-align: center;
    padding-top: 20vh;
    margin: 1em 4em;
    border-style: solid;
    border-color: black;
    border-width: 1px;
    border-radius: 5px;
    flex: 1;
    padding-top: 0em;
    padding-bottom: 3em;
    padding-left: 2em;
    padding-right: 2em;
    background-color: rgba(0, 0, 0, 0.5);
  }

  h1 {
    padding: 1em;
    text-align: center;
  }

  p {
    font-size: 1.2em;
  }

  @media screen and (max-width: 425px) {
    main {
      margin: 1em 1em;
    }
  }
</style>
