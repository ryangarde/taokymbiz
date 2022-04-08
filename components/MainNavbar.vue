<template>
	<div class="navbar">
		<nuxt-img class="logo" src="/logo.webp" fit="cover" width="205" height="80" />

		<div class="actions">
			<div class="links">
				<template v-for="link in links">
					<NuxtLink :to="link.url" class="link" v-if="!link.children">{{ link.label }}</NuxtLink>
					<template v-else-if="link.children">
						<div class="link-dropdown">
							<NuxtLink :to="link.url" class="link">
								{{ link.label }}
								<div class="arrow"></div>
							</NuxtLink>
							<div class="link-dropdown-menu-wrapper">
								<div class="link-dropdown-menu">
									<template v-for="child in link.children">
										<NuxtLink :to="child.url" class="dropdown-link">
											{{ child.label }}
										</NuxtLink>
									</template>
								</div>
							</div>
						</div>
					</template>
				</template>
			</div>

			<div class="buttons">
				<Button backgroundColor="#f10000" small borderRadius="6px">BOOK DEMO</Button>
				<Button backgroundColor="#f10000" small borderRadius="6px">CALL NOW</Button>
				<Button backgroundColor="#f10000" small borderRadius="6px">MORE INFO</Button>
			</div>
		</div>
	</div>
</template>

<script>
import Button from './inputs/Button.vue';

export default {
	components: { Button },
	data: () => ({
		links: [
			{ label: 'Home', url: '/' },
			{ label: 'About', url: '/about' },
			{
				label: 'Services',
				url: '/services',
				children: [
					{ label: 'Appointment Setting', url: '/appointment-setting' },
					{ label: 'Virtual Assistance', url: '/virtual-assistance' },
					{ label: 'Leads', url: '/leads' },
					{ label: 'Digital Marketing', url: '/digital-marketing' },
					{ label: 'Web Hosting', url: '/web-hosting' },
					{ label: 'My Account', url: '/my-account' },
				],
			},
			{
				label: 'Resources',
				url: '/resources',
				children: [
					{ label: 'Case Study', url: '/case-study' },
					{ label: 'Resource Center', url: 'resource-center' },
					{ label: 'FAQ', url: 'faq' },
				],
			},
			{ label: 'Contact', url: '/contact' },
		],
	}),
};
</script>

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

.actions {
	display: flex;
	column-gap: 15px;
	align-items: center;
}

.links {
	display: flex;
}

.link {
	display: flex;
	align-items: center;
	column-gap: 12px;
	position: relative;
	font-weight: bold;
	font-size: 18px;
	padding: 7px 15px;
	cursor: pointer;
	transition: 0.3s color;
}

.link::after {
	content: '';
	position: absolute;
	left: 0;
	right: 0;
	bottom: 0;
	height: 3px;
	background-color: #fff;
	opacity: 0;
	transition: 0.3s opacity;
}

.link:hover {
	color: #fff;
}

.link:hover::after {
	opacity: 1;
}

.link:hover .arrow {
	border-color: #fff transparent transparent transparent;
}

.buttons {
	display: flex;
	align-items: center;
	column-gap: 10px;
}

.link-dropdown {
	position: relative;
}

.link-dropdown:hover .link {
	color: #fff;
}

.link-dropdown:hover .arrow {
	border-color: #fff transparent transparent transparent;
}

.link-dropdown:hover .link::after {
	opacity: 1;
}

.link-dropdown:hover .link-dropdown-menu-wrapper {
	opacity: 1;
	pointer-events: all;
}

.link-dropdown-menu-wrapper {
	position: absolute;
	left: 0;
	top: 100%;
	padding-top: 20px;
	opacity: 0;
	transition: 0.3s;
	pointer-events: none;
}

.link-dropdown-menu {
	display: flex;
	flex-direction: column;
	background-color: #fff;
	border-radius: 20px;
	font-size: 18px;
	font-weight: 500;
	box-shadow: 0px 0px 10px 0px var(--clr-primary-main);
}

.dropdown-link {
	white-space: nowrap;
	font-family: Arial;
	padding: 10px 30px;
}

.dropdown-link:hover {
	color: var(--clr-primary-main);
	transition: 0.2s;
}

.arrow {
	width: 0;
	height: 0;
	border-width: 7px 7px 0 7px;
	border-color: black transparent transparent transparent;
	border-style: solid;
	transition: 0.3s;
}
</style>
