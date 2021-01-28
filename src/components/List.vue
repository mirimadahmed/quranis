<template>
  <div class="row text-left">
    <div v-for="surah in surahs" :key="surah.number" class="col-2">
      {{ surah.number }}. {{ surah.nameEnglish }}
    </div>
  </div>
</template>

<script>
export default {
  props: {
    surahs: {
      type: Array,
      required: true,
    },
  },
};
</script>

<style></style>
