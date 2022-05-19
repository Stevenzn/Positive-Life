<template>
  <div class="form">
      <h2>Log In</h2>
    <form @submit.prevent="submit" class="login-form">
      <input required v-model="username" type="text" placeholder="Username" />
      <input required v-model="password" type="password" placeholder="Password" />
      <button>login</button>
      <p class="message">Not registered? <router-link to="/register">Create Account</router-link> </p>
    </form>
  </div>
   <div data-aos="flip-up" class="reg-pag">
    <a class="reg-pag-link" href="#reg"><i class="fa-solid fa-arrow-up"></i></a>
  </div>
</template>

<script>
export default {
  data() {
    return {
      password: "",
      username: "",
    };
  },
  methods: {
    submit() {
      console.log(this.password, this.username);
    },
  },
  name: "Login",
  components: {},
};
</script>

<style lang="scss">
h2{
    font-size: 2rem;
    font-weight: bold;
    color: var(--rosado);
    margin-bottom: 1rem;
}
.form {
  max-width: 360px;
  margin: 1rem auto 12rem;
  padding: 45px;
  text-align: center;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2), 0 5px 5px 0 rgba(0, 0, 0, 0.24);
}
.form input {
  font-family: "Roboto", sans-serif;
  outline: 0;
  width: 100%;
  border: none;
  border-bottom: 2px solid #f69fcb;
  margin: 0 0 15px;
  padding: 15px;
  font-size: 14px;
}

.form input:focus{
border-bottom: var(--rosado) 2px solid;
}

.form button {
  text-transform: uppercase;
  outline: 0;
  background: var(--rosado);
  width: 50%;
  border: 0;
  padding: 15px;
  color: #ffffff;
  font-size: 14px;
  -webkit-transition: all 0.3 ease;
  transition: all 0.3 ease;
  cursor: pointer;
  border-radius:0.5rem;
}
.form button:hover,
.form button:active,
.form button:focus {
  background: var(--morado);
}
.form .message {
  margin: 15px 0 0;
  font-size: 15px;
}
.message a {
  color: var(--rosado);
  text-decoration: none;
}

.message a:hover {
  text-decoration: underline;
}
</style>
