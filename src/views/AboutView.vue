<template>
  <Nav></Nav>
  <div class="about-container">
    <h1>This is an about page</h1>
  </div>
  <Footer></Footer>
  <router-view></router-view>

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
