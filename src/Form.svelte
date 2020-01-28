<script>
    export let firstName = "";
</script>

<h2 class:welcome={firstName}>Welcome, {firstName}</h2>
<input bind:value={firstName}>

<style>
  .welcome {
    color: orangered
  }
</style>
