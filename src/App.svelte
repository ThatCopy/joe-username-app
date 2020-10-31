<script lang="ts">
import { generate } from "joe-username";

let name = generate();

function handleClick() {
	name = generate();
}

</script>

<main>
	<h1 id="heading">Joe Username Generator</h1>
	<h2>{name}</h2>
	<button on:click={handleClick}>Generate</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
	#heading{
		font-size: 300%;
	}
</style>