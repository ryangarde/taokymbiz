<template>
	<button class="button" :class="{ block, small }" :style="{ backgroundColor, fontSize, borderRadius }"><slot /></button>
</template>

<script>
export default {
	props: {
		block: {
			type: Boolean,
			default: false,
		},
		small: {
			type: Boolean,
			default: false,
		},
		color: {
			type: String,
		},
		fontSize: {
			type: String,
		},
		borderRadius: {
			type: String,
		},
		color: {
			type: String,
		},
	},

	data: () => ({
		backgroundColor: '',
	}),

	created() {
		if (this.color === 'theme-red') {
			this.backgroundColor = '#f10000';
		} else {
			this.backgroundColor = this.color;
		}
	},
};
</script>

<style>
.button {
	background-color: var(--clr-primary-main);
	color: #fff;
	padding: 10px 25px;
	border: none;
	border-radius: 4px;
	font-size: 14px;
	font-weight: 600;
}

.button.block {
	width: 100%;
}

.button.small {
	font-size: 11px;
	padding: 10px 22px;
}
</style>
