<script>
  let show = true;

  let hideAlert = () => {
      show = false;
  }
</script>

{#if show}
  <div class="alert">50% off 
      <button on:click={hideAlert}>Hide</button>
  </div>
{/if}

<style>
  .alert {
    padding: 8px;
    font-size: 18px;
    background-color: darkseagreen;
    color: darkslategrey;
  }
</style>
