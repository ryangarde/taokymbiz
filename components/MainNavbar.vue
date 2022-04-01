<template>
	<div class="navbar">
		<img class="logo" src="@/assets/logo.webp" />

		<div class="actions">
			<div class="links">
				<div class="link">Home</div>
				<div class="link">About</div>
				<div class="link">Services</div>
				<div class="link">Resources</div>
				<div class="link">Contact</div>
			</div>

			<div class="buttons">
				<button>BOOK DEMO</button>
				<button>CALL NOW</button>
				<button>MORE INFO</button>
			</div>
		</div>
	</div>
</template>

<style scroped>
.navbar {
	position: fixed;
	top: 0;
	left: 0;
	display: flex;
	justify-content: space-between;
	align-items: center;
	width: 100%;
	background-color: var(--clr-primary-main);
	height: 80px;
	padding: 0 95px;
}

.logo {
	height: 100%;
}

.actions {
	display: flex;
	column-gap: 15px;
	align-items: center;
}

.links {
	display: flex;
	column-gap: 25px;
}

.link {
	font-weight: bold;
	font-size: 18px;
}

.buttons {
	display: flex;
	column-gap: 10px;
}

.buttons button {
	background-color: #f10000;
	color: #fff;
	padding: 12px 28px;
	border: none;
	border-radius: 6px;
	font-size: 11px;
	font-weight: 600;
}
</style>
