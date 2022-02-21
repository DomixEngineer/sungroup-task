<template>
  <section>
    <div class="container">
      <ul class="pretty-list">
        <li v-for="listItem in listItems">{{ listItem }}</li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "prettyList.vue",
  props: {
    listItems: Array
  }
}
</script>

<style scoped>
@font-face {
  font-family: 'Lato-Light';
  src: url(../../assets/fonts/Lato-Light.ttf);
}
.header {
  color: #000000;
  font-family: "Lato-Light";
  font-size: 50px;
  text-align: left;
  line-height: 60px;
}
.container {
  max-width: 1321px;
  width: 100%;
  margin: 0 auto;
}
.pretty-list {
  list-style-type: none;
  font-family: "Lato-Light";
  font-size: 20px;
  line-height: 30px;
}
</style>
