<script>
import AppLogo from './AppLogo.vue';

export default {
    name: "FooterComponent",
    components: {
        AppLogo
    }
}
</script>

<template>
    <footer>
		<div class="container">
        	<div class="footer-cols">
				<div>
					<AppLogo />	
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
@use "../assets/scss/partials/layout" as *;

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