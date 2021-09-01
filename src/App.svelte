<script>
  import Form from "./Form.svelte";

  let foods = [
    { name: "Apple", color: "Red", id: 0 },
    { name: "Carrot", color: "Orange", id: 1 },
  ];

  const addFood = (e) => {
    foods = [e.detail, ...foods];
  };
</script>

<main>
  <Form on:addFood={addFood} />
  {#each foods as food (food.id)}
    <div class="fooditem">
      <h3>{food.name}</h3>
      <p>Color: {food.color}</p>
    </div>
  {/each}
</main>

<style>
  .fooditem {
    border: 2px solid gray;
    text-align: left;
    padding: 8px;
    margin-top: 20px;
    width: 100%;
  }

  main {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>
