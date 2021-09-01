<script>
  export let btnText = "default texxt";
</script>

<div class="card" on:click|self>
  <span> Click to log </span>
  <button on:click|once={() => console.log("once")}>{btnText}</button>
</div>

<!-- markup (zero or more items) goes here -->
<style>
  .card {
    padding: 12px;
    border: 1px solid violet;
    color: white;
  }
  button {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: lightblue;
  }
</style>
