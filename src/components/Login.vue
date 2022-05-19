<template>
  <div class="form">
    <form @submit.prevent="submit" method="post">
      <div class="form-group">
        <input type="email" class="form-control" id="email" v-model="email" placeholder="Email">
      </div>
      <div class="form-group">
        <input type="password" class="form-control" id="password" v-model="password" placeholder="Password">
      </div>
      <button type="submit" class="btn">Log In</button>
    </form>
  </div>
</template>

<script>
export default {
    data() {
        return {
        email: "",
        password: '',
        };
    },
    methods: {
        submit() {
        this.$store.dispatch("login", {
            email: this.email,
            password: this.password,
        });
        },
    },
    name: "Login",
    components: {},
}
</script>

<style lang="scss" scoped>
.form{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 50vh;
    margin: 0 auto;
    padding: 2rem 0;
}
</style>