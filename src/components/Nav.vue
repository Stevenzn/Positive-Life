<template>
  <header>
    <div class="logo-container">
      <figure><img src="@/assets/LogoPositiveLife.png" alt="" /></figure>
    </div>
    <nav class="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About us</router-link>
      <router-link to="/login">login</router-link>
    </nav>
  </header>

</template>

<script>
export default {
  data() {
    return {};
  },
  name: "Nav",
  components: {},
};
</script>

<style lang="scss" scoped>
header {
  width: 100%;
  height: 15vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
}
.logo-container {
  width: 30%;

  figure {
    width: 70%;
    margin: 0;
  }

  img {
    width: 100%;
  }
}

.nav {
  margin: 0 1rem 0 0;
  width: 40%;
  display: flex;
  justify-content: space-around;
  font-size: 1rem;
  font-weight: bold;
  }
/* EXTRA*/
@media screen and (min-width: 500px) {
  .logo-container {
    width: 25%;
  }
  .nav {
    width: 40%;
  }
}

/* TABLET */
@media screen and (min-width: 580px) {
  .logo-container {
  width: 20%;
  figure {
    width: 80%;
  }
  .nav{
    width:35%;
  }
}
}
/* PC */
@media screen and (min-width: 768px) {
  .logo-container {
    width: 15%;
  }
  .nav {
    width: 30%;
  }
}
/* LARGE SCREEN */
@media screen and (min-width: 990px) {
.logo-container {
    width: 12%;
  }
  .nav {
    width: 25%;
  }
}
</style>
