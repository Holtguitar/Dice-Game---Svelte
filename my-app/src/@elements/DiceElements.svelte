<script context="module">
	// Dice Elements, structured as classes.
	class Dice {
		constructor(id, faceValue, hidden, faded) {
			this.id = id;
			this.faceValue = faceValue;
			this.diceEL = `./src/static/dice-${this.faceValue}.png`;
			this.hidden = hidden;
			this.faded = faded;
		}
	}

	export const dice0 = new Dice(0, 1, true, false);
	export const dice1 = new Dice(1, 2, true, false);
	export const dice2 = new Dice(2, 3, true, false);
	export const dice3 = new Dice(3, 4, true, false);
	export const dice4 = new Dice(4, 5, true, false);
	export const dice5 = new Dice(5, 6, true, false);
	export const diceSets = [dice0, dice1, dice2, dice3, dice4, dice5];
</script>

<diceElements>
	<img src={dice0.diceEL} alt="Playing dice" class="dice0" />
	<img src={dice1.diceEL} alt="Playing dice" class="dice1" />
	<img src={dice2.diceEL} alt="Playing dice" class="dice2" />
	<img src={dice3.diceEL} alt="Playing dice" class="dice3" />
	<img src={dice4.diceEL} alt="Playing dice" class="dice4" />
	<img src={dice5.diceEL} alt="Playing dice" class="dice5" />
</diceElements>

<style>
	.dice0 {
		position: absolute;
		left: 12.5%;
		top: 25rem;
		transform: translateX(-50%);
		height: 8rem;
		box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
	}
	.dice1 {
		position: absolute;
		left: 27.5%;
		top: 25rem;
		transform: translateX(-50%);
		height: 8rem;
		box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
	}

	.dice2 {
		position: absolute;
		left: 42.5%;
		top: 25rem;
		transform: translateX(-50%);
		height: 8rem;
		box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
	}
	.dice3 {
		position: absolute;
		left: 57.5%;
		top: 25rem;
		transform: translateX(-50%);
		height: 8rem;
		box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
	}
	.dice4 {
		position: absolute;
		left: 72.5%;
		top: 25rem;
		transform: translateX(-50%);
		height: 8rem;
		box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
	}
	.dice5 {
		position: absolute;
		left: 87.5%;
		top: 25rem;
		transform: translateX(-50%);
		height: 8rem;
		box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
	}

	.not--faded {
		opacity: 1;
	}

	.faded {
		opacity: 0.5;
	}

	.more-faded {
		opacity: 0.15;
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
</style>
