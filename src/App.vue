<template>
  <div id="app">
    <IndexHeader />
    <IndexContent />
    <IndexFooter />
  </div>
</template>

<script>
import IndexHeader from "./components/Header.vue";
import IndexContent from "./components/Content.vue";
import IndexFooter from "./components/IndexFooter.vue";

export default {
  name: "App",
  components: {
    IndexHeader,
    IndexContent,
    IndexFooter,
  },
};
</script>

<style lang="scss">
@import url(./assets/scss/partials/_common.scss);
</style>




