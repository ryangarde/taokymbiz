<template>
	<div class="root">
		<div class="body">
			<SectionTitle> FEATURES </SectionTitle>

			<ol class="pl-6">
				<li>
					<div class="font-bold"> UCaaS (Unified Communications as a Service) </div>
					<ul class="pl-12">
						<li>Blends internet-based phone and messaging into a full-featured communications platform.</li>
						<li>Companies adopt UCaaS to provide staff with collaboration tools to work anywhere.</li>
						<li>UCaaS solutions function across a user’s computer, desk phone, and smartphone.</li>
					</ul>
				</li>
				<br />
				<li class="mt-4">
					<div class="font-bold"> Pre-set Appointments & Transfers </div>
					<ul class="pl-12">
						<li>Discover and interact with your ideal consumer further along in your sales funnel.</li>
						<li>Accelerates sales, reduces CPA and increases the morale of your sales force.</li>
						<li>
							A warm transfer is a transferred call that has been screened using your value proposition and better prepared to speak with
							your sales representative.
						</li>
						<li>
							Pre-set appointments schedule a time, date for phone call or meeting. In many cases, we pre-populate these meetings directly
							to your calendar based on your availability.
						</li>
					</ul>
				</li>
			</ol>
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
	background-image: linear-gradient(160deg, #fff 1%, #3782f6 100%);
	color: #fff;
}

.body {
	width: 60%;
	margin: 0 auto;
	background-color: var(--clr-primary-dark);
	padding: 50px;
	border-radius: 30px;
}

ol {
	font-family: Calibri;
	font-size: 20px;
}
</style>
