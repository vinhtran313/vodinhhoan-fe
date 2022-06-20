<template>
  <div class="container">
	<img src="../static/logo.jpg" alt="" class="title">
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
          targets: '.title',
          translateX: 250,
          rotate: '1turn',
          backgroundColor: '#FFF',
          duration: 800
        })
      }
    }
  }
</script>
<style scoped>
	.container {
		width: 300px;
		height: auto;
	}
	.container img {
		max-width: 100%;
	}
</style>