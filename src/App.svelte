<script>
	let name = "Bro";
	let src = "favicon.png";

	const handleInput = (e) => {
		name = e.target.value;
	}

	const resetname = () => {
		name = "gasdfoasnifdiasf";
	}
</script>

<main>
	<h1>Hello {name} </h1>
	<input type="text" bind:value={name}>
	<button on:click={resetname}>Set name to unknown</button>
	<img {src} alt="favicon">
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