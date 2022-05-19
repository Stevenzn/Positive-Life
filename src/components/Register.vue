<template>
  <div class="form">
    <h2>Register</h2>
    <form @submit.prevent="submit">
        
      <input
        type="text"
        placeholder="Username"
        v-model="username"
        required
      />
      <input
        type="password"
        placeholder="Password"
        v-model="password"
        required
      />
      <button type="submit">Register</button>
        <p class="message">
            Already registered? <router-link to="/login">Login</router-link>
        </p>
    </form>
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

<style lang="scss" scoped>
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
  /* box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2), 0 5px 5px 0 rgba(0, 0, 0, 0.24); */
}
.form input {
  font-family: "Roboto", sans-serif;
  outline: 0;
  width: 100%;
  border: none;
  border-bottom: 2px solid var(--rosado);
  margin: 0 0 15px;
  padding: 15px;
  font-size: 14px;
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
