<template>
  <Nav></Nav>
  <h2>hola desde el login</h2>
  <Footer></Footer>
</template>

<script>
import Nav from "@/components/Nav.vue";
import Footer from "@/components/Footer.vue";
export default {
    data() {
        return {};
    },
    name: "login",
    components: {
        Nav,
        Footer,
    },
}
</script>

<style>

</style>