<template>
	<div class="footer">
		<div class="body">
			<section class="sections">
				<div>
					<div class="font-bold">CONTACT US</div>
					<div class="content">
						<div class="font-bold"> Phone </div>
						<div> +1 240-319-7019 </div>
						<div class="font-bold">Email</div>
						<div> sales@taokymbiz.com </div>
						<div class="font-bold">Address</div>
						<div> 14514 Bubbling Spring Rd, Boyds MD 20841 </div>
					</div>
				</div>

				<div>
					<div class="font-bold">JOIN OUR NEWSLETTER</div>
					<div class="content"> Sign up to receive timely, useful information in your inbox. </div>
					<button>SUBSCRIBE</button>
				</div>
				<div>
					<div class="font-bold">EMAIL US</div> <div class="content"> Get in touch with us, leave a message. </div>
					<button>EMAIL US</button>
				</div>
				<div>
					<div class="font-bold">SITE NAVIGATION</div>
					<div class="content">
						<div>Home</div>
						<div>About Us</div>
						<div>Services</div>
						<div>Resources</div>
						<div>Contact Us</div>
					</div>
				</div>
			</section>

			<div class="content text-center mt-5">
				<div> Copyright © 2022 Taokym Business Solutions </div>
				<div>Privacy Policy</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.footer {
	background-color: var(--clr-primary-dark);
	color: #fff;
	padding: 30px;
}

.body {
	width: 60%;
	margin: 0 auto;
}

.sections {
	display: flex;
	flex-wrap: wrap;
	gap: 20px;
}

.content {
	font-family: Calibri;
	font-size: 15px;
}

button {
	background-color: #f10000;
	color: #fff;
	padding: 9px 28px;
	border: none;
	border-radius: 6px;
	font-size: 13px;
	font-weight: 600;
}
</style>
