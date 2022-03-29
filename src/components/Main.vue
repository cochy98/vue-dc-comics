<template>
  <main>
    <MainContent />
    <MainNav />
  </main>
</template>

<script>
import MainContent from "./MainContent.vue";
import MainNav from "./MainNav.vue";

export default {
  name: "IndexMain",
  components: {
    MainContent,
    MainNav,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {
  color: white;
}
</style>
