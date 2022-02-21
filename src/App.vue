<template>
  <div id="app">
    <sections :sections="sections"></sections>
  </div>
</template>

<script>
import Sections from "./components/shared/Sections";
import sectionsData from './dataMockups/sections';

export default {
  name: 'App',
  components: {
    Sections,
  },
  data() {
    return {
      sections: sectionsData,
    }
  }
}
</script>

<style>
</style>
