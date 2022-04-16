<template>
	<div class="container">
		<SectionTitle> </SectionTitle>
	</div>
</template>

<script>
import SectionTitle from '~/components/typography/SectionTitle.vue';

export default {
	components: { SectionTitle },
	head() {
		return {
			title: 'About Us',
		};
	},
};
</script>
