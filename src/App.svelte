<script>
	import Nested from "./Nested.svelte";
</script>

<Nested answer={40}/>


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