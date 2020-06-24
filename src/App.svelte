<script>
  import Title from "./Title.svelte";
  import Each from "./Each.svelte";
  import Form from "./Form.svelte";
  import Computed from "./Computed.svelte";
  import Toggle from "./Toggle.svelte";

  const arr = [{ id: 1, name: "Carl" }, { id: 2, name: "Richard" }];
</script>

<Title />
<Each myArray={arr} />
<Form />
<Computed />
<Toggle />
