<template>
	<div>
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
import Appointment from '~/components/appointment-setting/Appointment.vue';
import WhyTaokym from '~/components/appointment-setting/WhyTaokym.vue';
import HowItWorks from '~/components/appointment-setting/HowItWorks.vue';
import Features from '~/components/appointment-setting/Features.vue';
import BusinessServed from '~/components/appointment-setting/BusinessServed.vue';

export default {
	components: { Appointment, WhyTaokym, HowItWorks, Features, BusinessServed },
	head() {
		return {
			title: 'Appointment Setting',
		};
	},
};
</script>
