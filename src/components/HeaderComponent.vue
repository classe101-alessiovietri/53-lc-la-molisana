<script>
import AppLogo from './AppLogo.vue';

export default {
    name: "HeaderComponent",
    components: {
        AppLogo
    }
}
</script>

<template>
    <header>
		<div class="container">
			<div class="center-all">
				<AppLogo />

				<ul>
					<li>
						<a href="#">
							Home
						</a>
					</li>
					<li>
						<a href="#" class="active">
							Prodotti
						</a>
					</li>
					<li>
						<a href="#">
							Chi Siamo
						</a>
					</li>
					<li>
						<a href="#">
							Contatti
						</a>
					</li>
				</ul>
			</div>
		</div>
    </header>
</template>

<style lang="scss" scoped>
.center-all {
	display: flex;
	flex-direction: column;
	align-items: center;
}

header {
	margin-bottom: 50px;

	> div {
		margin-bottom: 30px;
	}

	ul {
		display: flex;
		list-style: none;
		padding: 0;

		li {
			a {
				display: inline-block;
				padding: 15px;
				color: black;
				text-decoration: none;
				font-size: 1.3rem;
				transition: .2s all ease-in-out;

				&:hover,		// header ul li a:hover
				&.active {		// header ul li a.active -> selezione sull'elemento
					background-color: cadetblue;
				}

				// .active {		// header ul li a .active -> selezione sul figlio
				// 	background-color: cadetblue;
				// }
			}
		}
	}
}
</style>