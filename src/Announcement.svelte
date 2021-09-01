<script>
  let show = true;

  let hideAlert = () => {
      show = false;
  }
  
  let warning = false;
</script>

{#if show}
  <div class="alert" class:warning={warning}>50% off 
      <button on:click={hideAlert}>Hide</button>
  </div>
{/if}

<style>
    .warning {
        color: darkslategrey;
        background-color: red;
    }
</style>
