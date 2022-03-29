<template>
  <div id="app">
    <IndexHeader />
    <IndexMain />
    <IndexFooter />
  </div>
</template>

<script>
import IndexHeader from "./components/Header.vue";
import IndexMain from "./components/Main.vue";
import IndexFooter from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    IndexHeader,
    IndexMain,
    IndexFooter,
  },
};
</script>

<style lang="scss">
@import url(./assets/scss/partials/_common.scss);
</style>




