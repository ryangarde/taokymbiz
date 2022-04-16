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
}

.body {
	padding-top: calc(80px + 50px);
	padding-bottom: 100px;
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
