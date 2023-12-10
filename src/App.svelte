<script>
	export let name;
	const designation = "Software Engineer"
	const boldText = `<b>Bold Text</b>`
</script>

<main>
	<h1>Hello {name}! {designation}</h1>
	<div>{@html boldText}</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
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