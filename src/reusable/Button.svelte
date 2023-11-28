<script>
  import { createEventDispatcher } from 'svelte';

  export let disabled;

  const dp = createEventDispatcher();

  const customBtnClick = () => dp('cClick');

  let buttonProps = {
    class: [$$restProps.class],
  };
</script>

<button {disabled} on:click={customBtnClick} {...buttonProps}>
  <slot />
</button>

<style>
  button:disabled {
    opacity: 0.5;
  }

  button {
    text-transform: uppercase;
    font-weight: 700;
    font-size: 1em;
    padding: 0.25em 0.5em;
    border: solid 1px #ffffff77;
    border-radius: 10px;
    background: rgba(0, 0, 0);
    color: whitesmoke;
    transition-duration: 0.1s;
    cursor: pointer;
  }

  button:active {
    color: #444444;
  }

  button:hover {
    background: rgb(64, 64, 64);
    border: solid 1px #ffffff;
    filter: brightness(1.2);
    filter: contrast(1.1);
  }

  .info-button {
    padding-top: 0em;
    padding-bottom: 0.25em;
    margin-bottom: 0.5em;
  }
</style>
