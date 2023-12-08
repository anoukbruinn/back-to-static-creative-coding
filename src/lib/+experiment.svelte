<body>
	<h1>Freaky abstract gradient button</h1>
	

	<div class="container">
		<button class="btn btn1"> Sponsor now </button>
		<button class="btn btn2"> Sponsor now </button>
		<button class="btn btn3"> Sponsor now </button>
		<button class="btn btn4"> Sponsor now </button>
	</div>
</body>

<style>
	body {
		margin: 0;
		padding: 0;
		background: #f1f1f1;
	}
	h1 {
		font-style: italic;
		display: flex;
		justify-content: center;
	}

	.container {
		position: absolute;
		left: 50%;
		top: 50%;
		transform: translate(-50%, -50%);
		text-align: center;
	}

	button {
		color: black;
		font-weight: 800;
	}

	.btn {
		border: none;
		margin: 20px;
		padding: 24px;
		width: 220px;
		font-family: 'apercu pro', sans-serif;
		text-transform: uppercase;
		border-radius: 30px;
		cursor: pointer;
		background-size: 200%;
		transition: 0.6s;
	}

	.btn1 {
		background-image: linear-gradient(to left, #ffda1d, #3dbae1, #ffda1d);
	}

	.btn2 {
		background-image: linear-gradient(to left, #3dbae1, #ffda1d, #3dbae1);
	}

	.btn3 {
		color: white;
		background-image: linear-gradient(to left, #179446, #163a3a, #179446);
	}

	.btn4 {
		color: white;
		background-image: linear-gradient(to left, #163a3a, #179446, #163a3a);
	}

	.btn:hover {
		background-position: right;
	}
</style>
