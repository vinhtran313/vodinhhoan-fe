<template>
	<div class="home-wrapper">
		<div class="logo-fullwidth">
			<div class="logo-mask">
				<div class="logo-part-a">
					<img src="~static/logo-part-A.png" alt="">
				</div>
				<div class="logo-part-b">
					<img src="~static/logo-part-B.png" alt="">
				</div>
				<div class="logo-part-c">
					<img src="~static/logo-part-C.png" alt="">
				</div>
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
				targets: '.logo-part-a',
				easing: "easeOutExpo",
				duration: 7000,
				delay: 1000,
				left: ['5rem', 'calc(50% - 10rem)'],
				translateY: ['-50%', '-50%'],
				opacity: [0, 1],
				translateX: '-50%',
			})
			this.$anime({
				targets: '.logo-part-c',
				easing: "easeOutExpo",
				duration: 7000,
				delay: 1000,
				right: ['5rem', 'calc(50% - 20rem)'],
				opacity: [0, 1],
				translateY: ['-50%', '-50%'],
				translateX: '-50%',
			})
			this.$anime({
				targets: '.logo-part-b',
				easing: "easeOutExpo",
				duration: 7000,
				delay: 1000,
				top: ['150rem', '50%'],
				opacity: [0, 1],
				translateY: ['-50%', '-50%'],
			})
			this.$anime({
				targets: '.logo-mask',
				easing: "easeOutExpo",
				duration: 7000,
				delay: 1000,
				background: ['transparent', 'hsla(0, 0%, 0%, 0.3)']
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
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;
		position: relative;

		background-image: url('https://mir-s3-cdn-cf.behance.net/project_modules/1400_opt_1/76dfba143262861.627789f26f11d.jpg');
		background-repeat: no-repeat;
		background-size: cover;

		.logo-mask {
			width: 100%;
			height: 15rem;
			display: flex;
			justify-content: center;
			align-items: center;
			// background: $logo-mask-bg;
			position: relative;
		}

		.logo-part-a,
		.logo-part-b,
		.logo-part-c {
			width: 10rem;
			aspect-ratio: 1/1;
			position: absolute;

			img {
				max-width: 100%;
			}
		}

		.logo-part-a {
			opacity: 0;
			left: 5rem;
			top: 50%;
			transform: translateY(-50%);
		}

		.logo-part-c {
			opacity: 0;
			top: 50%;
			right: 5rem;
			transform: translateY(-50%);
		}

		.logo-part-b {
			opacity: 0;
			top: 1000rem;
			transform: translateY(-50%);
		}

	}
}
</style>