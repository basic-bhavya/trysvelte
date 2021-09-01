<script>
  import { createEventDispatcher } from "svelte";

  const dispatch = createEventDispatcher();
  let name, color;

  const handleSubmit = () => {
    const food = {
      name: name,
      color: color,
      id: Math.random(),
    };

    dispatch("addFood", food);
  };
</script>

<form on:submit|preventDefault={handleSubmit}>
  <input type="text" placeholder="name" bind:value={name} />
  <input type="text" placeholder="color" bind:value={color} />
  <button>Add Food</button>
</form>

<!-- markup (zero or more items) goes here -->
<style>
</style>
