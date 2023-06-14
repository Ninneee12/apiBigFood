<template>
  <div>
    <form @submit.prevent="realizarLogin">
      <input type="text" id="usuario" v-model="usuario" placeholder="Usuário" />
      <br />
      <input type="password" id="senha" v-model="senha" placeholder="Senha" />
      <br />
      <button type="submit">Login</button>
      <a href="#">Esqueceu sua senha?</a> <br />
      <a href="#">Fazer cadastro</a>
    </form>
  </div>
</template>

<script setup>
import { ref } from "vue";
const usuario = ref("");
const senha = ref("");
console.log("BASE: " + process.env.BASE_URL);

const realizarLogin = () => {
  if (usuario.value === "sofia" && senha.value === "sofia123") {
    alert("Login realizado com sucesso!");
  } else {
    alert("Usuario ou senha incorretos.");
  }
};
</script>

<style>
form {
  display: flex;
  flex-direction: column;
  width: 30%;
  margin: auto;
  margin-bottom: 35px;
  justify-content: center;
}

input {
  margin-top: 15px;
  height: 35px;
}

button {
  margin-top: 15px;
  height: 35px;
  width: 50%;
  transform: translate(50%);
  margin-bottom: 15px;
}
</style>
