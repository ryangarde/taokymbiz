<template>
	<div class="root">
		<MainNavbar />

		<main class="body">
			<Nuxt />
		</main>

		<MainFooter />
	</div>
</template>

<style scoped>
.root {
	display: flex;
	flex-direction: column;
	min-height: 100vh;
}

.body {
	display: flex;
	flex-direction: column;
	flex-grow: 1;
	padding-top: 80px;
}
</style>

<script>
import MainNavbar from '@/components/MainNavbar.vue';
import MainFooter from '@/components/MainFooter.vue';

export default {
	components: {
		MainNavbar,
		MainFooter,
	},
};
</script>
