<script>
	let num = 0
</script>

<main>
	{#if num === 0}
		<h2>Number is Zero</h2>
	{:else if num > 0}
		<h2>Number is Positive</h2>
	{:else if num < 0}
		<h2>number is Negative</h2>
	{:else}
		<h2>Not a Number</h2>
	{/if}
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