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
* {
	margin: 0;
	box-sizing: border-box;
	font-family: Arial, Helvetica, sans-serif;

	&:not(ul) {
		padding: 0;
	}
}

.container {
	max-width: 800px;
	margin: 0 auto;
}

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