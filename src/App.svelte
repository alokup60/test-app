<script>
	let count = 0

	const inc = () => {
		count +=1
	}
</script>

<main>
	<button on:click={inc}>
		Clicked {count}
		{count === 1 ? "time" :"times"}
		</button>
</main>

<style>
	button{
		background-color: rgb(38, 38, 129);
		color: white;
		border-radius: 8px;
		cursor: pointer;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>