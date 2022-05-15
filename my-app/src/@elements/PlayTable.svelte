<section class="player player--0">
	<h2 class="name" id="name--1" style="padding: 10px; border: 5px double rgb(6, 1, 46);">
		Player 1
	</h2>
	<p class="score" id="score--0">0</p>
	<div class="current">
		<p class="current-label">Current</p>
		<p class="current-score" id="current--0">0</p>
	</div>
</section>
<section class="player player--1">
	<h2 class="name" id="name--1" style="padding: 10px; border: 5px double rgb(6, 1, 46);">
		Player 2
	</h2>
	<p class="score" id="score--1">0</p>
	<div class="current">
		<p class="current-label">Current</p>
		<p class="current-score" id="current--1">0</p>
	</div>
</section>
<section class="player player--2 player">
	<h2 class="name" id="name--0" style="padding: 10px; border: 5px double rgb(6, 1, 46);">
		Player 3
	</h2>
	<p class="score" id="score--2">0</p>
	<div class="current">
		<p class="current-label">Current</p>
		<p class="current-score" id="current--2">0</p>
	</div>
</section>

<section class="player player--3 player">
	<h2 class="name" id="name--0" style="padding: 10px; border: 5px double rgb(6, 1, 46);">
		Player 4
	</h2>
	<p class="score" id="score--3">0</p>
	<div class="current">
		<p class="current-label">Current</p>
		<p class="current-score" id="current--3">0</p>
	</div>
</section>

<style>
	.player {
		position: relative;
		flex: 10%;
		padding: 1rem;
		display: absolute;
		flex-direction: column;
		align-items: center;
		transition: all 0.75s;
		/* width: max-content; */
	}

	/* ELEMENTS */
	.name {
		position: relative;
		font-size: 4rem;
		text-shadow: 2px 2px #160b58;
		color: #05021b;
		text-transform: uppercase;
		letter-spacing: 1px;
		word-spacing: 2px;
		font-weight: 300;
		margin-bottom: 1rem;
		/* background-color: #1a6be6; */
		box-shadow: 2px 2px rgb(36, 35, 35);
		border-radius: 9px;
	}

	.score {
		font-size: 5rem;
		font-weight: 300;
		color: #130106;
		margin-bottom: 20rem;
		margin-left: 10rem;
		margin-top: 2rem;
	}

	.player--active {
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
	}

	.player--active .name {
		font-weight: 600;
	}
	.player--active .score {
		font-weight: 400;
	}

	.player--active .current {
		opacity: 1;
	}

	.current {
		background-color: #252323;
		border: solid;
		border-color: #090136;
		opacity: 0.8;
		border-radius: 9px;
		color: rgb(255, 255, 255);
		width: 65%;
		padding: 0%;
		text-align: center;
		transition: all 0.75s;
		margin-left: 3rem;
	}

	.current-label {
		text-transform: uppercase;
		margin-bottom: 1rem;
		font-size: 1.7rem;
		color: #ddd;
		padding: 0%;
		text-decoration: underline;
	}

	.current-score {
		font-size: 3rem;
		padding: 0%;
	}

	.hidden {
		display: none;
	}

	/* ABSOLUTE POSITIONED ELEMENTS */

	.player--winner {
		background-image: linear-gradient(
			to top left,
			#484849,
			#110363,
			#5b5b5c,
			#04069b,
			#5a5a5c,
			#110363,
			#343435,
			#090136
		);
	}

	.player--winner .name {
		font-weight: 700;
		color: #0c2e61;
	}
</style>
