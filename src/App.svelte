<script>
  let name, num, isChecked, value, selected;
  let questions = [
    { id: 1, text: "What is hello" },
    { id: 2, text: "What is world" },
  ];
</script>

<main>
  <input type="text" bind:value={name} />
  <input type="number" bind:value={num} />
  <input type="checkbox" bind:value={isChecked} />

  <label>
    <input type="radio" bind:group={value} value={1} />
    1
  </label>
  <label>
    <input type="radio" bind:group={value} value={2} />
    2
  </label>
  <label>
    <input type="radio" bind:group={value} value={3} />
    3
  </label>

  <select bind:value={selected}>
    {#each questions as question}
      <option value={question}>{question.text}</option>
    {/each}
  </select>
</main>

<style>
  h5,
  p {
    margin: 4px 0px;
  }

  .card {
    padding: 8px;
    border-radius: 20px;
    border: 2px solid gray;
    min-width: 400px;
  }

  main {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  h1 {
    text-align: center;
  }
</style>
