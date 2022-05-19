<template>
  <Nav></Nav>
  <div class="about-container">
    <h2>Hola desde about</h2>
  </div>
  <Footer></Footer>
</template>

<script>
import Nav from "@/components/Nav.vue";
import Footer from '@/components/Footer.vue';
export default {
  name: 'AboutView',
  components: {
    Nav,
    Footer
}
}
</script>
