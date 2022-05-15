<rules>
	<div id="rules" class="modal-content hidden">
		<span class="close">&times;</span>
		<div class="modal-header">
			<h2>SCORING</h2>
		</div>
		<div class="modal-body">
			<h>
				<br />
				⚀ = 100<br />
				⚄ = 50<br />
				⚁ ⚁ ⚁ = 200<br />
				⚂ ⚂ ⚂ = 300<br />
				⚃ ⚃ ⚃ = 400<br />
				⚄ ⚄ ⚄ = 500<br />
				⚅ ⚅ ⚅ = 600<br />
				⚀ ⚁ ⚂ ⚃ ⚄ ⚅ = 750<br />
				⚀ ⚀ ⚀ ⚀ ⚀ ⚀ = 10,000<br />
				<br />
			</h>
		</div>
		<div class="modal-footer">
			<h>
				Combinations of more than 3<br />
				double the score with each<br />
				extra dice.<br />
				<br />
				First to get exactly 10,000 wins!
			</h>
		</div>
	</div>
</rules>

<style>
	.modal-header {
		padding: 2px 16px;
		text-align: center;
		background-image: linear-gradient(to top left, #c8c7ce, #e9e8f0, #b1b0b4, 0);
		color: rgb(7, 7, 7);
		margin-top: 0%;
		font-size: 0.8cm;
	}

	.modal-footer {
		padding: 2px 16px;
		text-align: center;
		background-image: linear-gradient(to top left, #c8c7ce, #e9e8f0, #b1b0b4, 0);
		color: rgb(7, 7, 7);
		margin-top: 0%;
		font-size: 0.6cm;
	}

	.modal-content {
		font-family: 'Nunito', sans-serif;
		font-size: 0.9cm;
		font-weight: 40;
		text-align: justify;
		height: 100vh;
		color: rgb(3, 0, 0);
		position: absolute;
		top: 50%;
		left: 87.5%;
		transform: translate(-50%, -50%);
		width: 20%;
		height: fit-content;
		background-image: linear-gradient(to top left, #c2c0c0, #ccc9c9, #f0eaea, #cecaca, #a5a1a1);
		padding: 1rem;
		border-radius: 10px;
		border-style: double;
		border-color: #022252;
		box-shadow: 0 3rem 5rem rgba(27, 5, 107, 0.3);
		z-index: 10;
	}
	.close-modal {
		top: 0.1rem;
		left: 1rem;
		font-size: 5rem;
		color: rgb(19, 1, 1);
		cursor: pointer;
		border: none;
		background: none;
	}

	.show-modal {
		font-size: 2rem;
		font-weight: 600;
		padding: 10px;
		margin: 5rem 2rem;
		border: none;
		background-color: #fff;
		color: #444;
		border-radius: 10rem;
		cursor: pointer;
	}

	.hidden {
		opacity: 0%;
	}
</style>
