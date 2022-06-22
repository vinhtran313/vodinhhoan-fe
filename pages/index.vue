<template>
	<div class="home-wrapper">
		<div class="logo-fullwidth">
			<div class="logo">
				<img src="~static/2.png" alt="">
			</div>
		</div>
	</div>
</template>

<script>
export default {
	mounted() {
		this.setAnimation()
	},

	methods: {
		setAnimation() {
			this.$anime({
				targets: '.logo',
				easing: "easeOutExpo",
				duration: 10000,
				delay: 1000,
				top: '50%',
				left: '50%',
				translateX: '-50%',
				translateY: '-50%',
				rotateX: '1turn',
			})
		}
	}
}
</script>
<style lang="scss">
@import "~assets/scss/variables.scss";

.home-wrapper {

	.logo-fullwidth {
		width: 100%;
		height: 1080px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: relative;

		background-image: url('https://mir-s3-cdn-cf.behance.net/project_modules/1400_opt_1/76dfba143262861.627789f26f11d.jpg');
		background-repeat: no-repeat;
		background-size: cover;

		.logo {
			width: 600px;
			background: transparent;
			position: absolute;
			top: 10%;
			left: 10%;

			img {
				max-width: 100%;
				background-color: transparent;
			}
		}

	}
}
</style>