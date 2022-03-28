<template>
  <div id="app">
    <!-- Header -->
    <IndexHeader />
    <!-- logo + Nav -->

    <!-- Main -->
    <IndexMain />
    <!-- Main Top -->
    <!-- Main Bottom -->

    <!-- Footer -->
    <IndexFooter />
    <!-- Footer top -->
    <!-- Footer bottom -->
  </div>
</template>

<script>
import IndexHeader from "./components/IndexHeader.vue";
import IndexMain from "./components/IndexHeader.vue";
import IndexFooter from "./components/IndexHeader.vue";

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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
