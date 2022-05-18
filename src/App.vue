<template>
  <router-view></router-view>
</template>

<script>
import Nav from "./components/Nav.vue";
import HomeView from "./views/HomeView.vue";
import AboutView from "./views/AboutView.vue";
import Footer from "./components/Footer.vue";
export default {
  data() {
    return {};
  },
  name: "App",
  components: {
    HomeView,
    AboutView,
    Nav,
    Footer
  },
};
</script>

<style lang="scss" scoped>

</style>
