<script>
	// import DiceElements from '../@elements/DiceElements.svelte';
	// import PlayTable from '../@elements/PlayTable.svelte';
	// import Rules from './rules.svelte';
	// import diceSets from '../@elements/DiceElements.svelte';
	import PlayTable from '../@elements/PlayTable.svelte';
	import DiceElements from '../@elements/DiceElements.svelte';
	import { diceRoll } from '../@rolling/DiceRoll.svelte';
</script>

<!-- svelte-ignore a11y-missing-attribute -->
<html>
	<body>
		<header>10,000 Dice Game</header>

		<div class="buttons">
			<button class="btn btn--new">🔄 New game</button>
			<button on:click={diceRoll} class="btn btn--roll">🎲 Roll dice</button>
			<button class="btn btn--hold">✋🏼 Hold</button>
			<button class="btn btn--steal">💎 Steal</button>
			<button class="btn btn--rules">📜 Rules</button>
		</div>

		<main>
			<PlayTable />
			<DiceElements />
		</main>
		<!-- <Rules /> -->
	</body>
</html>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: inherit;
	}

	html {
		font-size: 62.5%;
		box-sizing: border-box;
	}

	/* LAYOUT */
	main {
		position: relative;
		width: 100%;
		background-image: linear-gradient(to top left, #110363, #071d9b, #04069b, #071d9b, #110363);
		background-repeat: no-repeat;
		backdrop-filter: blur(200px);
		filter: blur();
		box-shadow: 5px 5px 5px rgb(43, 42, 42);
		border-color: #110363;
		border-style: groove;
		border-radius: 9px;
		overflow: hidden;
		display: flex;
	}

	header {
		position: fixed;
		top: 5%;
		left: 20%;
		font-size: 3.5rem;
		font-weight: bolder;
		color: rgb(10, 8, 99);
		text-shadow: 2px 3px 4px rgb(43, 42, 42);
	}

	body {
		font-family: 'Nunito', sans-serif;
		font-weight: 400;
		height: 100vh;
		color: rgb(3, 0, 0);
		background-image: linear-gradient(
			to top left,
			#6e6969,
			#a5a5a5,
			#bebdbd,
			#918f8f,
			#6e6c6c,
			#686767
		);

		display: flex;
		white-space: nowrap;
		padding: 0;
		align-items: center;
		justify-content: center;
	}

	.btn {
		position: absolute;
		left: 50%;
		transform: translateX(-50%);
		color: rgb(218, 218, 218);
		background-image: linear-gradient(
			to top left,
			#090136,
			#110363,
			#071d9b,
			#04069b,
			#071d9b,
			#110363,
			#090136
		);
		border: solid;
		border-color: #090136;
		font-family: inherit;
		font-size: 1.8rem;
		text-transform: uppercase;
		cursor: pointer;
		font-weight: 400;
		transition: all 0.2s;
		background-color: rgb(0, 0, 0);
		background-color: rgba(0, 0, 0, 0.6);
		backdrop-filter: blur(10px);
		padding: 0.7rem 2.5rem;
		border-radius: 50rem;
		box-shadow: 0 1.75rem 3.5rem rgba(0, 0, 0, 0.1);
	}

	.btn::first-letter {
		font-size: 2.4rem;
		display: inline-block;
		margin-right: 0.7rem;
	}

	.btn--new {
		top: 2%;
		left: 60%;
	}
	.btn--rules {
		top: 2%;
		left: 75%;
	}
	.btn--roll {
		top: 30%;
		left: 8%;
	}
	.btn--hold {
		top: 45%;
		left: 8%;
	}
	.btn--steal {
		top: 60%;
		left: 8%;
	}

	.btn:active {
		transform: translate(-50%, 1px);
		box-shadow: 0 1rem 1rem rgba(8, 19, 117, 0.884);
	}

	.btn:focus {
		outline: none;
	}
</style>
