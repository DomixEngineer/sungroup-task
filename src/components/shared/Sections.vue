<template>
  <div>
    <template v-for="section in sections.sections">
      <template v-if="section.type === 'image'">
        <div v-if="section.hasHeader" class="container">
          <h1 class="header">Specyfikacja</h1>
        </div>
        <single-image :img-src="section.src"></single-image>
      </template>
      <template v-if="section.type === 'section'">
        <single-section :title="section.title" :paragraphs="section.paragraphs"></single-section>
      </template>
      <template v-if="section.type === 'table_of_content'">
        <table-of-content :title="tableData.title" :rows="tableData.rows"></table-of-content>
      </template>
      <template v-if="section.type === 'list_items'">
        <pretty-list :list-items="section.items"></pretty-list>
      </template>
      <template v-if="section.type === 'fullpage_section'">
        <fullpage-section></fullpage-section>
      </template>
    </template>
  </div>
</template>

<script>
import singleSection from "./singleSection";
import singleImage from "./singleImage";
import tableOfContent from "./tableOfContent";
import tableData from '../../dataMockups/tableOfContent';
import prettyList from './prettyList'
import fullpageSection from "./fullpageSection";

export default {
  name: "Sections.vue",
  components: {
    singleSection,
    singleImage,
    prettyList,
    tableOfContent,
    fullpageSection
  },
  data() {
    return {
      tableData: tableData
    }
  },
  props: {
    sections: Array
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
</style>
