<template>
  <div class="site">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/macro/Header.vue";
import Main from "./components/macro/Main.vue";
import Footer from "./components/macro/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  created() {
    document.title = "Mattia Dominici | Front-end Developer";
  },
};
</script>

<style lang="scss">
@import "./assets/style/main.scss";
</style>
