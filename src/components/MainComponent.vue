<script>
export default {
    name: "MainComponent",
    data() {
        return {

        }
    },
    methods: {

    }
}
</script>

<template>
    <main>
		<div class="container">
			<h1>
				--] Content goes here [--
			</h1>
		</div>
    </main>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/layout" as *;

main {
	padding: 80px 0;
	background-image: url('../assets/img/fondo-pag-speciali.jpg');
	background-position: center;
	background-size: cover;
	background-repeat: no-repeat;

	h1 {
		color: blue;
		text-align: center;
	}
}
</style>