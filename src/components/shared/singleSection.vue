<template>
  <section class="container section">
    <h1 class="section-title">{{ title }}</h1>
    <p v-for="paragraph in paragraphs" class="section-paragraph">
      {{ paragraph }}
    </p>
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

<style scoped>
  @font-face {
    font-family: 'Lato-Light';
    src: url(../../assets/fonts/Lato-Light.ttf);
  }
  .section-title {
    color: #000000;
    font-family: "Lato-Light";
    font-size: 50px;
    text-align: left;
    line-height: 60px;
  }
  .section-paragraph {
    font-family: "Lato-Light";
    font-size: 20px;
    text-align: left;
    line-height: 30px;
    color: #000000;
  }
</style>
