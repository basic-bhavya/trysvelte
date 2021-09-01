<script>
  import Button from "./Button.svelte";

  const log = () => {
    console.log("clicked");
  };
</script>

<main>
  <Button on:click={log} btnText={"Component button"} />
  <button>App button</button>
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
