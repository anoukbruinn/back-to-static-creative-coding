<body>
	<link href="https://fonts.googleapis.com/css?family=Russo+One" rel="stylesheet" />

	<svg viewBox="0 0 1320 300">
		<text x="50%" y="0%" dy=".35em" text-anchor="middle">
			<a href="src/lib/+experiment.svelte">Experiment 1</a>
		</text>
		<text x="50%" y="50%" dy=".35em" text-anchor="middle">
			<a href="src/lib/+experiment2.svelte">Experiment 2</a>
		</text>
		<text x="50%" y="100%" dy=".35em" text-anchor="middle">
			<a href="src/lib/+experiment3.svelte">Experiment 3</a>
		</text>
	</svg>
</body>

<style>
	svg {
		font-family: 'Russo One', sans-serif;
		position: absolute;
		width: 100%;
		height: 100%;
		display: flex;
		justify-content: center;
	}

	text {
		display: flex;
		justify-content: center;
	}
	svg text {
		text-transform: uppercase;
		animation: stroke 5s infinite alternate;
		stroke-width: 2;
		stroke: #365fa0;
		font-size: 140px;
	}
	@keyframes stroke {
		0% {
			fill: rgba(72, 138, 20, 0);
			stroke: rgba(54, 95, 160, 1);
			stroke-dashoffset: 25%;
			stroke-dasharray: 0 50%;
			stroke-width: 2;
		}
		70% {
			fill: rgba(72, 138, 20, 0);
			stroke: rgba(54, 95, 160, 1);
		}
		80% {
			fill: rgba(72, 138, 20, 0);
			stroke: rgba(54, 95, 160, 1);
			stroke-width: 3;
		}
		100% {
			fill: rgb(204, 72, 180);
			stroke: rgba(54, 95, 160, 0);
			stroke-dashoffset: -25%;
			stroke-dasharray: 50% 0;
			stroke-width: 0;
		}
	}
</style>
