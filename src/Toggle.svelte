<script>
  import { fly, fade } from "svelte/transition";
  let visible = false;
</script>

<button on:click={() => (visible = !visible)}>Toggle</button>
{#if visible}
  <h1 in:fly={{ x: 300, duration: 3000 }} out:fade={{ duration: 2000 }}>
    Hi there! 💁🏽‍♂️
  </h1>
{/if}
