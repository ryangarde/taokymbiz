<template>
	<div class="root">
		<div class="body">
			<SectionTitle>HOW IT WORKS?</SectionTitle>

			<nuxt-img class="how-it-works-image mx-auto" src="/images/howit-works-appointment.webp" width="80%" fit="cover" />

			<div class="content">
				The Virtual Appointments Setter (VAS) will convert prospects into possible buyers. They will contact leads, prospects and clients
				using your company’s value proposition and set an appointment to your calendar or transfer the call. If you don’t have a value
				proposition and phone script, we can help you create one. If you don’t have prospects, we may be able to help there too!
			</div>

			<img src="@/assets/images/flow-appointment.webp" alt="" class="flow-appointment mx-auto" width="40%" fit="cover" />
		</div>
	</div>
</template>

<script>
import SectionTitle from '../typography/SectionTitle.vue';
export default {
	components: { SectionTitle },
};
</script>

<style scoped>
.root {
	padding: 100px;
}

.body {
	width: 60%;
	margin: 0 auto;
	text-align: center;
}

.how-it-works-image {
	margin-top: 20px;
}

.content {
	line-height: 1.6;
	font-family: Calibri;
	font-size: 20px;
	margin-top: 25px;
}

.flow-appointment {
	margin-top: 50px;
}
</style>
