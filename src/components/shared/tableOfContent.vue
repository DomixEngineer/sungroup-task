<template>
  <section class="container">
    <h1 class="section-title">{{ title }}</h1>
    <table class="tableOfContent">
      <tr v-for="row in rows">
        <td class="leftCol"><p>{{ row.rowTitle }}</p></td>
        <td>
          <p v-for="singleData in row.rowData">
            {{ singleData }}
          </p>
          <p v-if="row.annotation" class="annotation">{{ row.annotation }}</p>
        </td>
      </tr>
    </table>
  </section>
</template>

<script>
export default {
  name: "tableOfContent.vue",
  props: {
    title: String,
    rows: Array
  }
}
</script>

<style scoped>
  @font-face {
    font-family: 'Lato-Light';
    src: url(../../assets/fonts/Lato-Light.ttf);
  }
  .section-title {
    font-family: 'Lato-Light';
    font-size: 50px;
    line-height: 60px;
    text-align: left;
    color: #000000;
  }
  .tableOfContent {
    border-collapse: collapse;
    width: 100%;
  }
  .tableOfContent tr {
    border-bottom: 1px solid rgba(151, 151, 151, 0.3);
  }
  .tableOfContent tr p {
    font-family: 'Lato-Light';
    font-size: 20px;
    line-height: 30px;
    text-align: left;
  }
  .tableOfContent .leftCol {
    display: inline;
  }
  .tableOfContent .leftCol p {
    line-height: 0;
  }
  .annotation {
    opacity: 0.6;
    font-size: 16px !important;
    color: #000000;
  }
</style>
