<script>
  import Card from "./Card.svelte";
</script>

<main>
  <Card>
    <h3>This is on top</h3>
    <button slot="button">This is a button</button>
    <p slot="hello">This is card</p>
    <h3>This is on bottom</h3>
	<h4 slot="notfound">This doesn't show</h4>
  </Card>
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
