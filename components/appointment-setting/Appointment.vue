<template>
	<div class="root">
		<div class="body">
			<SectionTitle>APPOINTMENT SETTING & TRANSFERS</SectionTitle>

			<div class="sub-title"> Fill your calendar with appointments while you focus on revenue generating tasks. </div>

			<div class="content">
				Appointment setting is one of the most difficult aspects of business development and one of the most common roadblocks for sales
				growth. It is a critical task that requires focus and tremendous activity to convert a prospect or client into an appointment or
				meeting.
			</div>

			<div class="appointments">
				<div class="appointment">
					<nuxt-img src="/icons/why-taokym.webp" width="218" height="221" />
					<Button block>Why TAOKYM?</Button>
				</div>
				<div class="appointment">
					<nuxt-img src="/icons/how-it-works-appointment.webp" width="218" height="221" />
					<Button block>How it Works?</Button>
				</div>
				<div class="appointment">
					<nuxt-img src="/icons/features.webp" width="218" height="221" />
					<Button block>Features</Button>
				</div>
				<div class="appointment">
					<nuxt-img src="/icons/industries-served.webp" width="218" height="221" />
					<Button block>Who We Serve?</Button>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import SectionTitle from '../typography/SectionTitle.vue';
import Button from '../inputs/Button.vue';
export default {
	components: { SectionTitle, Button },
};
</script>

<style scoped>
.root {
	display: flex;
	justify-content: center;
	align-items: center;
	text-align: center;
	min-height: calc(100vh - 80px);
}

@media screen and (min-width: 1280px) {
	.body {
		width: 60%;
	}
}

.title {
	font-size: 30px;
	font-weight: 600;
}

.sub-title {
	font-size: 26px;
	font-weight: 600;
	margin-top: 20px;
}

.content {
	margin-top: 30px;
	font-size: 20px;
	line-height: 1.6;
	font-family: Calibri;
	margin-bottom: 40px;
}

.appointments {
	display: flex;
	flex-wrap: wrap;
	margin: -20px;
}

.appointment {
	width: 25%;
	padding: 10px;
}

.appointment img {
	/* width: 80%; */
	margin: 0 auto;
	margin-bottom: 25px;
}
</style>
