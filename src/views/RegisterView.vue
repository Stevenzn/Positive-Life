<template>
    <Nav></Nav>
    <Register></Register>
     <div data-aos="flip-up" class="reg-pag">
    <a class="reg-pag-link" href="#reg"><i class="fa-solid fa-arrow-up"></i></a>
  </div>
    <Footer></Footer>
</template>

<script>
import Nav from "@/components/Nav.vue";
import Footer from '@/components/Footer.vue';
import Register from "@/components/Register.vue";
export default {
    data() {
        return {};
    },
    name: "RegisterView",
    components: {
    Nav,
    Footer,
    Register
},
}
</script>

<style>

</style>