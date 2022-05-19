<template>
  <router-view></router-view>
</template>

<script>
import Nav from "./components/Nav.vue";
import HomeView from "./views/HomeView.vue";
import AboutView from "./views/AboutView.vue";
import Footer from "./components/Footer.vue";
import LoginView from "./views/LoginView.vue";
export default {
  data() {
    return {};
  },
  name: "App",
  components: {
    AboutView,
    Nav,
    Footer,
    HomeView,
    LoginView,
  },
};
</script>

<style lang="scss" scoped></style>
