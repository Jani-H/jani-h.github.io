<script>
  import Router from 'svelte-spa-router';

  import Home from '../core/Home.svelte';
  import About from '../core/About.svelte';
  import Contact from '../core/Contact.svelte';
  import Works from '../core/Works.svelte';

  const routes = {
    '/': Home,
    '/about': About,
    '/contact': Contact,
    '/projects': Works,
  };
</script>

<main>
  <Router {routes} />
</main>

<style>
  main {
    padding-bottom: 5em;
  }
</style>
