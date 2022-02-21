<template>
  <div class="container">
    <img :src="resolveImgUrl(imgSrc)" :alt="imgAlt" class="single-image">
  </div>
</template>

<script>
export default {
  name: "singleImage.vue",
  props: {
    imgSrc: String,
    imgAlt: String
  },
  methods: {
    resolveImgUrl(imgSrc) {
      let images = require.context('../../assets/images/', false, /\.png$|\.jpg$/)
      return images('./' + imgSrc);
    }
  }
}
</script>

<style scoped>
  .single-image {
    max-width: 1321px;
    width: 100%;
    display: block;
    margin: 55px auto;
  }
</style>
