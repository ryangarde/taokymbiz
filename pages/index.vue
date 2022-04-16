<template>
	<div class="root container">
		<v-row class="text-center mt-4">
			<v-col md="4" class="flex flex-col justify-between">
				<div>
					<nuxt-img src="/images/home/mission.webp" width="170" class="logo" />
					<SectionTitle>MISSION</SectionTitle>

					<article class="content">We empower our partners to grow their organizations and improve their quality of life.</article>
				</div>

				<div>
					<Button color="theme-red" borderRadius="8px" class="rounded-0">BOOK DEMO</Button>
				</div>
			</v-col>

			<v-col md="4" class="flex flex-col justify-between">
				<div>
					<nuxt-img src="/images/home/how-we-work.webp" width="170" class="logo" />
					<SectionTitle>HOW WE WORK</SectionTitle>

					<article class="content">
						We partner with quality professionals where cost of labor is fair and the desire for success is high. Our business model creates
						a systematic structure of oversight, accountability and supports both off-shore and on-shore, establishing clear expectations
						with our clients and delivering on our promises!
					</article>
				</div>

				<div>
					<Button color="theme-red" borderRadius="8px">CALL NOW</Button>
				</div>
			</v-col>

			<v-col md="4" class="flex flex-col justify-between gap-8">
				<div>
					<nuxt-img src="/images/home/what-we-do.webp" width="170" class="logo" />
					<SectionTitle>WHAT WE DO</SectionTitle>

					<article class="content">
						We are an innovative resource supplier across industries providing high-value and affordable resources for multiple business
						needs at a fixed hourly rate. Our resources have produced marketing material, logos, outbound calling, inbound call center
						support, lead generation, administrative support, and more. If you have a requirement for work that can be done remotely we can
						staff, support, and create redundancy for that opportunity.
					</article>
				</div>

				<div>
					<Button color="theme-red" borderRadius="8px">MORE INFO</Button>
				</div>
			</v-col>
		</v-row>
	</div>
</template>

<script>
import SectionTitle from '~/components/typography/SectionTitle.vue';
import Button from '~/components/inputs/Button';

export default {
	components: { SectionTitle, Button },

	head() {
		return {
			title: 'Home',
		};
	},
};
</script>

<style scoped>
.root {
	padding: 0 4%;
}

.logo {
	margin: 0 auto;
}

.content {
	font-family: Calibri;
	line-height: 1.6;
	font-size: 20px;
}
</style>
