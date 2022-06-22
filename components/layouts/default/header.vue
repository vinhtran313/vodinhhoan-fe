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

<style scoped>
.main-header {
	height: 40px;

	display: flex;
	align-items: center;
	justify-content: center;

	background: rgba(255, 255, 255, .35);
}
</style>