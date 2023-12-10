<script>
	let names = ["Alok","Bruce","Anil"]
</script>

<main>
	{#each names as name,index}
	<h2>{index +1}{name}</h2>
	{/each}
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	.success{
		color: green;
	}

	.danger {
		color: red;
	}

	h1 {
		color: #ff3e00;
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