<script>
  import Router from './utils/Router.svelte';
  import Header from './core/Header.svelte';
  import Navbar from './core/Navbar.svelte';
  import Footer from './core/Footer.svelte';
</script>

<main>
  <Header />
  <Navbar />
  <Router />
  <Footer />
</main>

<style>
  :global(:root) {
    background-color: #222222;
    background-image: url('https://jani-h.github.io/jani-h.github.io/images/background.png');
    background-repeat: repeat;
    background-size: 256px 256px;
  }
</style>
