<script>
  import { onMount } from "svelte";
  let food = 0;
  let rent = 0;

  onMount(() => {
    food = 10;
    rent = 1000;
  });

  $: totalExpense = food + rent; // $ is called destiny operator
  /*
    Angular:: get totalExpense() {
        return this.food + this.rent
    }
    Vuejs:: computed: {
        totalExpense: function() {
            return this.food + this.rent;
        }
    }
    Reactjs + Mobx:: @computed get totalExpense(){
        return this.food + this.rent;
    }
*/
</script>

<h2>Total expense: €{totalExpense}</h2>

<button on:click={() => (food += 10)}>INCREASE</button>
<button on:click={() => (food -= 10)}>LESSEN</button>
