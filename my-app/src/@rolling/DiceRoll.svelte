<script context="module">
	import { diceSets } from '../@elements/DiceElements.svelte';

	export const diceRoll = () => {
		for (let i = 0; i < diceSets.length; i++) {
			let diceElement = document.querySelector(`.dice${diceSets[i].id}`);
			let diceVal = Math.trunc(Math.random() * 6) + 1;
			diceElement.src = `./src/static/dice-${diceVal}.png`;
		}
	};
</script>
