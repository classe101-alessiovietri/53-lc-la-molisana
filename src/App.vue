<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
    name: "App",
    components: {
		HeaderComponent,
		MainComponent,
		FooterComponent,
    },
};
</script>

<template>

	<HeaderComponent />

	<MainComponent />

	<FooterComponent />

</template>

<style lang="scss">
@use "./assets/scss/partials/reset" as *;
</style>
