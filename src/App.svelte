<script>
	let firstname = "";
	let lastname = "";

	$: fullname = `${firstname} ${lastname}`;
	$: console.log(lastname);
</script>

<main>
	<h1>Hello {fullname} </h1>
	<label for="firstname">firstname</label>
	<input type="text" bind:value={firstname}>
	<label for="firstname">Lastname</label>
	<input type="text" bind:value={lastname}>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	h1 {
		text-align: center;
	}
</style>