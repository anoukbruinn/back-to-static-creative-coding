<body>
	<h1>Where the real legends begin</h1>

	<div id="main" class="m1">
		<div id="r1"></div>
		<div id="r2"></div>
		<div id="r3"></div>
		<div id="r4"></div>
	</div>

	<style>
		@import url('https://fonts.googleapis.com/css2?family=Creepster&display=swap');
		h1 {
			color: lightpink;
			display: flex;
			justify-content: center;
			align-items: center;
			margin-top: 25rem;
			margin-bottom: auto;
			font-family: creepster;
			font-size: 9rem;

			opacity: 0;
			animation: lightson 0.5s ease 3 forwards;
		}

		@keyframes lightson {
			0% {
				opacity: 0;
				text-shadow:
					0px 0px 0px #fe1dad,
					0px 0px 0px #fe1dad,
					0px 0px 0px #fe1dad;
			}
			20% {
				opacity: 0.5;
				text-shadow:
					0px 0px 2.5px #fe1dad,
					0px 0px 5px #fe1dad,
					1px 1px 25px #fe1dad;
			}
			40% {
				opacity: 0;
				text-shadow:
					0px 0px 1px #fe1dad,
					0px 0px 2px #fe1dad,
					0px 0px 10px #fe1dad;
			}
			50% {
				opacity: 1;
				text-shadow:
					0px 0px 5px #fe1dad,
					0px 0px 10px #fe1dad,
					1px 1px 50px #fe1dad;
			}
			100% {
				opacity: 1;
				text-shadow:
					0px 0px 5px #fe1dad,
					0px 0px 10px #fe1dad,
					1px 1px 50px #fe1dad;
			}
		}

		.blackpink span {
			transform: scaleX(-1);
			display: inline-block;
		}
		.blackpink__tagline {
			text-align: right;
			font-size: 0.8rem;
		}
		body {
			margin: 0;
			-webkit-transition: 2s linear;
			-moz-transition: 2s linear;
			-ms-transition: 2s linear;
			-o-transition: 2s linear;
			transition: 2s linear;
		}

		#main {
			width: 500px;
			height: 500px;
			top: 50%;
			left: 50%;
			margin: -250px 0 0 -250px;
			position: absolute;
			filter: blur(20px) contrast(500%);
			-webkit-animation: rotate 10s linear infinite;
			-moz-animation: rotate 10s linear infinite;
			-ms-animation: rotate 10s linear infinite;
			-o-animation: rotate 10s linear infinite;
			animation: rotate 10s linear infinite;
		}

		#r1,
		#r2,
		#r3,
		#r4 {
			width: 150px;
			height: 150px;
			position: absolute;
		}

		#r1 {
			top: 100px;
			left: 100px;
		}

		#r2 {
			top: 100px;
			left: 250px;
			-webkit-transform: rotateY(180deg);
			-moz-transform: rotateY(180deg);
			-ms-transform: rotateY(180deg);
			-o-transform: rotateY(180deg);
			transform: rotateY(180deg);
		}

		#r3 {
			top: 250px;
			left: 100px;
			-webkit-transform: rotateX(180deg);
			-moz-transform: rotateX(180deg);
			-ms-transform: rotateX(180deg);
			-o-transform: rotateX(180deg);
			transform: rotateX(180deg);
		}

		#r4 {
			top: 250px;
			left: 250px;
			-webkit-transform: rotateX(180deg) rotateY(180deg);
			-moz-transform: rotateX(180deg) rotateY(180deg);
			-ms-transform: rotateX(180deg) rotateY(180deg);
			-o-transform: rotateX(180deg) rotateY(180deg);
			transform: rotateX(180deg) rotateY(180deg);
		}

		.circle {
			background: #000;
			width: 25px;
			height: 25px;
			top: 140px;
			left: 140px;
			border: 3px solid #fff;
			border-radius: 100px;
			opacity: 0;
			position: absolute;
			-webkit-animation: rotate 1s linear infinite;
			-moz-animation: rotate 1s linear infinite;
			-ms-animation: rotate 1s linear infinite;
			-o-animation: rotate 1s linear infinite;
			animation: rotate 1s linear infinite;
			-webkit-transition: 0.5s linear;
			-moz-transition: 0.5s linear;
			-ms-transition: 0.5s linear;
			-o-transition: 0.5s linear;
			transition: 0.5s linear;
		}

		@-webkit-keyframes rotate {
			0% {
				-webkit-transform: scale(1.8) rotate(0deg);
			}
			100% {
				-webkit-transform: scale(1.8) rotate(360deg);
			}
		}

		@-moz-keyframes rotate {
			0% {
				-moz-transform: scale(1.8) rotate(0deg);
			}
			100% {
				-moz-transform: scale(1.8) rotate(360deg);
			}
		}

		@-ms-keyframes rotate {
			0% {
				-ms-transform: scale(1.8) rotate(0deg);
			}
			100% {
				-ms-transform: scale(1.8) rotate(360deg);
			}
		}

		@-o-keyframes rotate {
			0% {
				-o-transform: scale(1.8) rotate(0deg);
			}
			100% {
				-o-transform: scale(1.8) rotate(360deg);
			}
		}

		@keyframes rotate {
			0% {
				transform: scale(1.8) rotate(0deg);
			}
			100% {
				transform: scale(1.8) rotate(360deg);
			}
		}
	</style>

	<script>
		var nbrCircle = 4;
		var cmpt = 0;
		while (cmpt < nbrCircle) {
			document.getElementById('r1').innerHTML =
				document.getElementById('r1').innerHTML + '<div class="circle"></div>';
			document.getElementById('r1').getElementsByClassName('circle')[cmpt].style.margin = '0 0 0 0';
			setTimeout(function () {
				document.getElementById('r1').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
			}, 500);
			document.getElementById('r2').innerHTML =
				document.getElementById('r2').innerHTML + '<div class="circle"></div>';
			document.getElementById('r2').getElementsByClassName('circle')[cmpt].style.margin = '0 0 0 0';
			setTimeout(function () {
				document.getElementById('r2').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
			}, 500);
			document.getElementById('r3').innerHTML =
				document.getElementById('r3').innerHTML + '<div class="circle"></div>';
			document.getElementById('r3').getElementsByClassName('circle')[cmpt].style.margin = '0 0 0 0';
			setTimeout(function () {
				document.getElementById('r3').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
			}, 500);
			document.getElementById('r4').innerHTML =
				document.getElementById('r4').innerHTML + '<div class="circle"></div>';
			document.getElementById('r4').getElementsByClassName('circle')[cmpt].style.margin = '0 0 0 0';
			setTimeout(function () {
				document.getElementById('r4').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
			}, 500);
			cmpt++;
		}
		setTimeout(function () {
			var cmpt = 0;
			while (cmpt < nbrCircle) {
				document.getElementById('r1').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
				document.getElementById('r2').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
				document.getElementById('r3').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
				document.getElementById('r4').getElementsByClassName('circle')[cmpt].style.opacity = '0.5';
				cmpt++;
			}
		}, 1000);
		setInterval(function () {
			linearMargin = false;
			var cmpt = 0;
			while (document.getElementById('r1').getElementsByClassName('circle')[cmpt]) {
				if (cmpt % 2 == 0) {
					linearMargin = false;
				} else {
					linearMargin = true;
				}
				var circle = document.getElementById('r1').getElementsByClassName('circle')[cmpt];
				var value1_1 = Math.floor(Math.random() * 255 + 0);
				var value1_2 = Math.floor(Math.random() * 255 + 0);
				var value1_3 = Math.floor(Math.random() * 255 + 0);
				var marginInterval = 100;
				var contentSize = 500;
				if (
					parseInt(circle.style.marginTop) + marginInterval < contentSize &&
					parseInt(circle.style.marginTop) + -marginInterval >= 0
				)
					var value2_1 =
						parseInt(circle.style.marginTop) +
						Math.floor(Math.random() * marginInterval + -marginInterval);
				else if (parseInt(circle.style.marginTop) + marginInterval < document.body.offsetHeight)
					var value2_1 =
						parseInt(circle.style.marginTop) + Math.floor(Math.random() * marginInterval + 0);
				else
					var value2_1 =
						parseInt(circle.style.marginTop) + -Math.floor(Math.random() * marginInterval + 0);
				if (linearMargin == true) value2_2 = value2_1;
				else if (
					parseInt(circle.style.marginLeft) + marginInterval < contentSize &&
					parseInt(circle.style.marginWidth) + -marginInterval >= 0
				)
					var value2_2 =
						parseInt(circle.style.marginLeft) +
						Math.floor(Math.random() * marginInterval + -marginInterval);
				else if (parseInt(circle.style.marginLeft) + marginInterval < document.body.offsetHeight)
					var value2_2 =
						parseInt(circle.style.marginLeft) + Math.floor(Math.random() * marginInterval + 0);
				else
					var value2_2 =
						parseInt(circle.style.marginLeft) + -Math.floor(Math.random() * marginInterval + 0);
				var value3_1 = Math.floor(Math.random() * 100 + 10);
				var value3_2 = value3_1;
				var value4_1 = Math.floor(Math.random() * 100 + 0);
				circle.style.background = 'rgb(' + value1_1 + ',' + value1_2 + ',' + value1_3 + ')';
				circle.style.margin = value2_1 + 'px 0 0 ' + value2_2 + 'px';
				circle.style.width = value3_1 + 'px';
				circle.style.height = value3_2 + 'px';
				circle.style.borderRadius = value4_1 + 'px';
				var circle = document.getElementById('r2').getElementsByClassName('circle')[cmpt];
				circle.style.background = 'rgb(' + value1_1 + ',' + value1_2 + ',' + value1_3 + ')';
				circle.style.margin = value2_1 + 'px 0 0 ' + value2_2 + 'px';
				circle.style.width = value3_1 + 'px';
				circle.style.height = value3_2 + 'px';
				circle.style.borderRadius = value4_1 + 'px';
				var circle = document.getElementById('r3').getElementsByClassName('circle')[cmpt];
				circle.style.background = 'rgb(' + value1_1 + ',' + value1_2 + ',' + value1_3 + ')';
				circle.style.margin = value2_1 + 'px 0 0 ' + value2_2 + 'px';
				circle.style.width = value3_1 + 'px';
				circle.style.height = value3_2 + 'px';
				circle.style.borderRadius = value4_1 + 'px';
				var circle = document.getElementById('r4').getElementsByClassName('circle')[cmpt];
				circle.style.background = 'rgb(' + value1_1 + ',' + value1_2 + ',' + value1_3 + ')';
				circle.style.margin = value2_1 + 'px 0 0 ' + value2_2 + 'px';
				circle.style.width = value3_1 + 'px';
				circle.style.height = value3_2 + 'px';
				circle.style.borderRadius = value4_1 + 'px';
				cmpt++;
			}
		}, 500);
		setInterval(function () {
			var value1 = Math.floor(Math.random() * 255 + 0);
			var value2 = Math.floor(Math.random() * 255 + 0);
			var value3 = Math.floor(Math.random() * 255 + 0);
			document.body.style.background = 'rgb(' + value1 + ',' + value2 + ',' + value3 + ')';
		}, 2000);
	</script>
</body>
