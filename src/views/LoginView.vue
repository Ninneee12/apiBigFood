<template>
    <main>
        <form @submit.prevent="realizarLogin">
        <input type="text" id="usuario" v-model="usuario" placeholder="Usuário" />
        <br />
        <input type="password" id="senha" v-model="senha" placeholder="Senha" />
        <br />
        <button type="submit">Login</button>
        <a href="#">Fazer cadastro</a>
        <a href="#">Esqueceu sua senha?</a> <br />
        </form>
    </main>
</template>

<script setup>
import { ref } from "vue";
import SimpleInput from "@/components/SimpleInput.vue"

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

<style scoped>

main{
    height: 70vh;
    display: flex;
    align-items: center;
}

form {
    display: flex;
    flex-direction: column;
    width: 30%;
    margin-bottom: 35px;
    justify-content: center;
    align-items: center;
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
