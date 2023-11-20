<script>
  import { push } from 'svelte-spa-router';
</script>

<nav>
  <ul>
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-missing-attribute -->
    <a on:click={() => push('/')}>Home</a>
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-missing-attribute -->
    <a on:click={() => push('/about')}>About</a>
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-missing-attribute -->
    <a on:click={() => push('/works')}>Works</a>
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <!-- svelte-ignore a11y-missing-attribute -->
    <a on:click={() => push('/contact')}>Contact</a>
  </ul>
</nav>

<style>
  nav {
    display: flex;
    justify-content: center;
    list-style: none;
    background-color: rgba(0, 0, 0, 0.75);
  }

  a {
    font-size: 1.25em;
    padding: 0em 1em;
  }
</style>
