<script>
export default {
    name: "FooterComponent",
    data() {
        return {

        }
    },
    methods: {

    }
}
</script>

<template>
    <footer>
		<div class="container">
        	<div class="footer-cols">
				<div>
					<img src="../assets/img/la-molisana-logo.png" alt="La Molisana">	
				</div>

				<div>
					<h4>
						Pastificio
					</h4>
					<ul>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
					</ul>
				</div>

				<div>
					<h4>
						Prodotti
					</h4>
					<ul>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
						<li>
							<a href="#">
								Link
							</a>
						</li>
					</ul>
				</div>
			</div>
		</div>
    </footer>
</template>

<style lang="scss" scoped>
* {
	margin: 0;
	box-sizing: border-box;
	font-family: Arial, Helvetica, sans-serif;

	&:not(ul) {
		padding: 0;
	}
}

img {
	width: 100%;
}

.container {
	max-width: 800px;
	margin: 0 auto;
}

footer {
	padding-bottom: 200px;
	background-image: url('../assets/img/footer-montagne-bottom.jpg');
	background-position: bottom center;
	background-repeat: no-repeat;
	background-size: 100% auto;
	margin-top: 50px;

	.footer-cols {
		display: flex;

		> * {
			width: calc(100% / 3);
		}
	}

	h4 {
		text-transform: uppercase;
		font-size: 1.4rem;
		margin-bottom: 15px;
		color: cadetblue;
	}

	ul {
		list-style: none;
		padding: 0;

		li {
			a {
				display: inline-block;
				padding: 5px 0;
				color: black;
			}
		}
	}
}
</style>