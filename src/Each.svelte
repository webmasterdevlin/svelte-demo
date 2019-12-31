<script>
    export let myArray;
</script>
{#if myArray.length > 0}
  {#each myArray as obj, i}
    <h3 key={obj.id}>{i + 1}. {obj.name}</h3>
  {/each}
 {:else}
  <h2>Empty</h2>
{/if}
