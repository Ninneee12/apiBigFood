<template>
    <section class="login">
        <div>
            <form>
                <input type="text" name="nome" placeholder="Nome de Usuário" id="login">
                <input type="password" name="senha" placeholder="Senha" id="password">
                <button @click="logar()">Entrar</button>
            </form>
            <a href="*">Esqueceu sua senha?</a>
        </div>
    </section>
    </template>
    <script> 

    import LoginPage from '../components/LoginPage.vue'

    export default {
    name: 'LoginView',
    components: {
        LoginPage
    }
    }

    function logar(){
        let login = document.getElementsById('login').value;
        let password = document.getElementById('password').value;

        if(
            login == "sofia@gmail" && password == "sofia123"){
                alert('Logado com sucesso')
            }
        else {
            alert('Usuário ou senha incorretos')
        }
    }

    </script>

    <style scoped>
    


*{
    margin: 0;
    padding: 0;
}

.login {
    display: flex;
    height: 100vh;
    justify-content: center;
    align-items: center;    
}

.login img{
    width: 90px;
    margin-bottom: 30px;
}

div {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 420px;
    height: 470px;
    border-radius: 10px;
}

form {
    display: flex;
    width: 100%;
    flex-direction: column;
}

input{
    margin: 20px;
    background-color: rgb(255, 255, 255);
    height: 50px;
    border: 1px solid black;
    border-radius: 10px;
    padding-left: 10px;
}

input:focus{
    border: 1px solid rgba(188, 72, 255, 0.671);
}

input::placeholder {
    font-weight: 200;
}

button{
    background-color: rgb(255, 128, 0);
    margin-top: 15px;
    margin-bottom: 15px;
    cursor: pointer;
    height: 55px;
    width: 200px;
    margin-left: 100px;
    color: white;
    font-weight: 300;
    font-size: 18px;
    padding-right: 10px;
    border-radius: 10px;
    border: none;
}


a{
    text-decoration: none;
    color: rgb(122, 122, 122);
    font-weight: 200;
}

a:hover {
    font-weight: 300;
}
</style>