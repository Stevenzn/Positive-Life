<template>
  <div class="form">
    <h2>Register</h2>
    <form @submit.prevent="submit">
      <input type="text" placeholder="Nombres" />
      <input type="text" placeholder="Apellidos" />
      <input type="number" placeholder="Numero" />
      <input type="text" placeholder="Pais" />
      <input type="text" placeholder="Depatamento" />
      <input type="text" placeholder="Ciudad" />
      <select name="Seleccionar" id="">
        <option value="">Selecciona una opcion</option>
        <option value="">Eres perra?1</option>
        <option value="">Eres perra?2</option>
      </select>
      <button type="submit">Register</button>
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

<style lang="scss" >
select{
  margin: 1rem 0;
  width: 60%;
}
/* h2{
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
} */
</style>
