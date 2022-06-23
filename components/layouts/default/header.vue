<template>
	<div class="main-header">
		<div class="phone-number">
			<a href="tel:+84984755975">0984-755-975</a>
		</div>
		<div class="social-icon">
			<a href="#">
				<font-awesome-icon :icon="['fab', 'facebook']" />
			</a>
		</div>
		<div class="social-icon">
			<a href="#">
				<font-awesome-icon :icon="['fab', 'instagram']" />
			</a>
		</div>
		<div class="social-icon">
			<a href="#">
				<font-awesome-icon :icon="['fab', 'pinterest-p']" />
			</a>
		</div>
	</div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "~assets/scss/variables.scss";

.main-header {
	height: 3rem;
	width: 100%;
	position: absolute;
	top: 0;
	left: 0;
	display: flex;
	align-items: center;
	justify-content: center;
	z-index: 1;

	background: $header-bg;
	transition: all 0.2s ease-in-out;

	a {
		color: $header-item-color;
		text-decoration: none;
		font-size: 1rem;
		transition: all 0.2s ease-in-out;
		font-weight: bold;
		background: transparent;

		&:hover {
			color: $header-item-color__on-hover;
		}
	}

	&:hover {
		a {
			color: $header-item-color__on-header-hover;

			&:hover {
				color: $header-item-color__on-hover;
			}
		}

		background: $header-bg-hover;
	}

	.phone-number {
		font-weight: bold;
		letter-spacing: .1rem;
		margin-right: .5rem;
		padding: .5rem;
	}

	.social-icon {
		margin: 0 .25rem;
		padding: .25rem;

		&:last-child {
			margin: 0 0 0 .25rem;
		}

		a {
			font-size: 1.25rem;
		}
	}
}
</style>