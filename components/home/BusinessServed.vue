<template>
	<div class="root">
		<div class="body">
			<SectionTitle>BUSINESSES SERVED</SectionTitle>
			<ul class="font-bold mb-14">
				<li>Any sales organization.</li>
				<li>Any business that has an appointment schedule that needs to be populated.</li>
			</ul>

			<v-expansion-panels class="panels" accordion tile>
				<v-expansion-panel class="panel">
					<v-expansion-panel-header class="panel-header"> 1. Insurance</v-expansion-panel-header>
					<v-expansion-panel-content class="panel-content" eager>
						<ul class="ml-8 p-4">
							<li>Agents</li>
							<li>Agencies</li>
							<li>Marketing Organizations</li>
							<li>Carriers</li>
						</ul>
					</v-expansion-panel-content>
				</v-expansion-panel>

				<v-expansion-panel class="panel">
					<v-expansion-panel-header class="panel-header">2. Health and Well-being</v-expansion-panel-header>
					<v-expansion-panel-content class="panel-content" eager>
						<ul class="ml-8 p-4">
							<li>Medical Professionals</li>
							<li>Medical Clinics</li>
							<li>Medical Equipment Wholesalers</li>
							<li>Spas</li>
						</ul>
					</v-expansion-panel-content>
				</v-expansion-panel>

				<v-expansion-panel class="panel">
					<v-expansion-panel-header class="panel-header">3. Professional Service</v-expansion-panel-header>
					<v-expansion-panel-content class="panel-content" eager>
						<ul class="ml-8 p-4">
							<li>Accountant</li>
							<li>Financial Advisors</li>
							<li>Financial Firms</li>
							<li>Lawyers</li>
						</ul>
					</v-expansion-panel-content>
				</v-expansion-panel>

				<v-expansion-panel class="panel">
					<v-expansion-panel-header class="panel-header">4. Fitness and Lifestyle</v-expansion-panel-header>
					<v-expansion-panel-content class="panel-content" eager>
						<ul class="ml-8 p-4">
							<li>Salons</li>
							<li>Fitness Instructors</li>
							<li>Personal Trainers</li>
						</ul>
					</v-expansion-panel-content>
				</v-expansion-panel>
			</v-expansion-panels>
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
	background-image: linear-gradient(20deg, #fff 1%, #3782f6 100%);
	color: #fff;
}

.body {
	width: 60%;
	margin: 0 auto;
	background-color: var(--clr-primary-dark);
	padding: 50px;
	border-radius: 30px;
}

ul {
	font-family: Calibri;
	font-size: 20px;
}

.panels {
	border-bottom: 1.5px solid #fff;
}

.panel {
	background-color: unset !important;
	color: #fff;
	border: 1.5px solid #fff;
	border-bottom: none;
}

.panel::before {
	box-shadow: unset;
}

.panel-header {
	border-bottom: 1.5px solid #fff;
	font-family: Roboto;
	font-size: 20px;
	font-weight: 600;
	flex-direction: row-reverse;
	justify-content: flex-end;
	column-gap: 15px;
}

/deep/.panel-header i {
	font-weight: 600;
	color: #fff !important;
}

.panel-content {
	/* padding: 20px; */
}
</style>
