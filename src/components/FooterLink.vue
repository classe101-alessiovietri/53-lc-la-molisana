<script>
export default {
    name: "FooterLink",
	props: {
		url: String,
		label: String
	}
}
</script>

<template>
	<li>
		<a :href="url">
			{{ label }}
		</a>
	</li>
</template>

<style lang="scss" scoped>
li {
	&.footer-link {
		a {
			color: red;
		}
	}

	a {
		display: inline-block;
		padding: 5px 0;
		color: black;
	}
}
</style>