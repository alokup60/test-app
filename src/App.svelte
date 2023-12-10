<script>
	let nums = [1,2,3,4];

	function addNum (){
		nums = [...nums,nums.length + 1] 
	}

	$: sum = nums.reduce((acc,curr) => acc+curr,0)
</script>

<main>

	<p>{nums.join(' + ')} = {sum}</p>

	<button on:click={addNum}>
		Add Numbers
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