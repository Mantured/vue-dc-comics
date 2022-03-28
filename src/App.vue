<template>
  <div id="app">
    <!-- Header -->
    <Header />
    <!-- logo + Nav -->

    <!-- Main -->
    <Main />
    <!-- Main Top -->
    <!-- Main Bottom -->

    <!-- Footer -->
    <Footer />
    <!-- Footer top -->
    <!-- Footer bottom -->
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
/* google font Montserrat & Raleway */
@import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;1,100&family=Raleway:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
/* collegamento style scss */
@import "./assets/scss/style.scss";
</style>
