<script>
    export let firstName = "";
</script>

<h2 class:welcome={firstName}>Welcome to NDC London, {firstName}</h2>
<input bind:value={firstName}>

<style>
  .welcome {
    color: orangered
  }
</style>