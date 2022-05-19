<template>
  <Nav></Nav>
  <Login></Login>
  <Footer></Footer>
</template>

<script>
import Nav from "@/components/Nav.vue";
import Footer from "@/components/Footer.vue";
import Login from "@/components/Login.vue";

export default {
    data() {
        return {};
    },
    name: "login",
    components: {
    Nav,
    Footer,
    Login
},
}
</script>

<style>

</style>