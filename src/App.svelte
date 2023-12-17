<script>
	import Counter from "./lib/Counter.svelte";

	import Button from "./lib/Button.svelte";
	import FaAngellist from "svelte-icons/fa/FaAngellist.svelte";

	let name = "Svelte";

	const props = {
		maxCount: 10,
		initialCount: 5
	};
</script>

<main>
	<h1>Hello {name.toLowerCase()}</h1>

	<Counter {...props} />

	<Button size="small" shadow>
		<div style:width="20px" slot="leftContent"><FaAngellist /></div>
		Button Text
	</Button>
</main>

<style>
	h1 {
		color: red;
	}
</style>
