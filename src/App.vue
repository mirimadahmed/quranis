<template>
  <div id="app" class="container">
    <p class="display-2">Quranis</p>
    <p class="display-4">The simplest Quran App you'll ever need</p>
    <List :surahs="surahs" />
  </div>
</template>

<script>
import { surahs } from "./data/surah";
import List from "./components/List.vue";

export default {
  name: "App",
  components: {
    List,
  },
  data() {
    return {
      surahs: surahs,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
