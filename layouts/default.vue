<template>
	<div class="body-wrapper">
		<LayoutsDefaultHeader></LayoutsDefaultHeader>
		<Nuxt />
	</div>
</template>

<script>

</script>

<style lang="scss">
@import "~assets/scss/variables.scss";

.body-wrapper {
	background-color: $layout-bg;
	min-height: 100vh;
	font-family: 'Helvetica';
}
</style>