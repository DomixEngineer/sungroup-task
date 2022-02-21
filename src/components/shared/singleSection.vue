<template>
  <section class="section">
    <h1 class="section__title">{{ title }}</h1>
  </section>
</template>

<script>
export default {
  name: "singleSection",
  data() {
    return {

    }
  },
  methods: {

  },
  props: {
    title: String,
    paragraphs: Array
  }
}
</script>

<style lang="scss" scoped>
  @font-face {
    font-family: 'Lato-Light';
    src: url(../../assets/fonts/Lato-Light.ttf);
  }
  .section {
    &__title {

     }
  }
</style>
