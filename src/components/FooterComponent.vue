<script>
import AppLogo from './AppLogo.vue';
import FooterLink from './FooterLink.vue';

export default {
    name: "FooterComponent",
    components: {
        AppLogo,
		FooterLink
    },
	data() {
		return {
			columnTwoLinks: [
				{
					url: '#',
					label: 'Link 1',
				},
				{
					url: '#',
					label: 'Link 2',
				},
				{
					url: '#',
					label: 'Link 3',
				},
				{
					url: '#',
					label: 'Link 4',
				},
				{
					url: '#',
					label: 'Link 5',
				},
				{
					url: '#',
					label: 'Link 6',
				},
			],
			columnThreeLinks: [
				{
					url: '#',
					label: 'Link A',
				},
				{
					url: '#',
					label: 'Link B',
				},
				{
					url: '#',
					label: 'Link C',
				},
				{
					url: '#',
					label: 'Link D',
				},
				{
					url: '#',
					label: 'Link E',
				},
				{
					url: '#',
					label: 'Link F',
				},
			]
		};
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
						<FooterLink
							v-for="(singleLink, index) in columnTwoLinks" :key="index"
							:url="singleLink.url"
							:label="singleLink.label" />
					</ul>
				</div>

				<div>
					<h4>
						Prodotti
					</h4>
					<ul>
						<FooterLink class="footer-link"
							v-for="(singleLink, index) in columnThreeLinks" :key="index"
							:url="singleLink.url"
							:label="singleLink.label" />
					</ul>
				</div>
			</div>
		</div>
    </footer>
</template>

<style lang="scss" scoped>
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
	}
}
</style>