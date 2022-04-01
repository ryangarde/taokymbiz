<template>
	<div class="root">
		<div class="body">
			<div class="title">APPOINTMENT SETTING & TRANSFERS</div>

			<div class="sub-title"> Fill your calendar with appointments while you focus on revenue generating tasks. </div>

			<div class="content">
				Appointment setting is one of the most difficult aspects of business development and one of the most common roadblocks for sales
				growth. It is a critical task that requires focus and tremendous activity to convert a prospect or client into an appointment or
				meeting.
			</div>

			<div class="appointments">
				<div class="appointment">
					<img src="@/assets/icons/why-taokym.webp" />
					<button>Why TAOKYM?</button>
				</div>
				<div class="appointment">
					<img src="@/assets/icons/how-it-works-appointment.webp" />
					<button>How it Works?</button>
				</div>
				<div class="appointment">
					<img src="@/assets/icons/features.webp" />
					<button>Features</button>
				</div>
				<div class="appointment">
					<img src="@/assets/icons/industries-served.webp" />
					<button>Who We Serve?</button>
				</div>
			</div>
		</div>
	</div>
</template>

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
	width: 80%;
	margin: 0 auto;
	margin-bottom: 25px;
}

.appointment button {
	background-color: var(--clr-primary-main);
	color: #fff;
	padding: 14px 28px;
	border: none;
	border-radius: 4px;
	font-size: 15px;
	font-weight: 600;
	width: 100%;
}
</style>
