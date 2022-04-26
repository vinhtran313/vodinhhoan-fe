<template>
  <div class="container">
    <div class="home-main">
      <div class="hero">
        <img
          src="https://mir-s3-cdn-cf.behance.net/project_modules/fs/15d6e3142122971.6260db8166020.png"
          alt="hero"
          class="hero-img"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
};
</script>
<style>
.hero {
  max-height: 100vh;
  object-fit: contain;
}
.hero img {
  width: 100%;
  max-height: 100%;
}
</style>
