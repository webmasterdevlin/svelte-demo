<script>
  import Form from './Form.svelte';
  import Each from './Each.svelte';
  import Toggle from './Toggle.svelte';
  const arr = [{id:1,name:'Carl'},{id:2,name:'Richard'}];
</script>
  <Toggle />
  <Form />
  <Each myArray={arr} />

