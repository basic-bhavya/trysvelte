<script>
  export let btnText = "default texxt";
</script>

<div>
  <span on:click> Click to log </span>
  <button>{btnText}</button>
</div>

<!-- markup (zero or more items) goes here -->
<style>
  button {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: lightblue;
  }
</style>
