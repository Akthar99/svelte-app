<script>
	let firstName = "Hasiru";
	let lastName = "Pinsara";
	let nameColor = "red";
	let version = 1.0;
	$: fullName = `${firstName} ${lastName}`;

	const handleClick = () => {
		
	}
	

</script>

<main>
	<h1 style="color : { nameColor }" >Hello { fullName } - { nameColor } !</h1>
	<p>Wellcome to my website . version : {version}</p>
	<button on:click={ handleClick }>Change Name</button>
	<input type="text" bind:value = { firstName }>
	<input type="text" bind:value = { lastName }>
	<input type="text" bind:value = { nameColor }>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {

		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>