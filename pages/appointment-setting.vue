<template>
	<div class="root">
		<Appointment />
		<WhyTaokym />
		<HowItWorks />
		<Features />
		<BusinessServed />
	</div>
</template>

<style scoped>
.root {
	flex-grow: 1;
}
</style>

<script>
import Appointment from '@/components/home/Appointment.vue';
import WhyTaokym from '~/components/home/WhyTaokym.vue';
import HowItWorks from '../components/home/HowItWorks.vue';
import Features from '~/components/home/Features.vue';
import BusinessServed from '../components/home/BusinessServed.vue';

export default {
	data() {
		return {
			form: {
				FirstName: 'fasef',
			},
		};
	},
	components: { Appointment, WhyTaokym, HowItWorks, Features, BusinessServed },
};
</script>
