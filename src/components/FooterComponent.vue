<template>
    <footer>
        <div class="logo">
            <img src="../assets/bar.png" alt="logo do app Sabor di Botequim">
            <h3>
                O maior concurso de butecos do Brasil!
            </h3>
            <a href="#">Veja como funciona</a>
            <p>© Todos os direitos reservados</p>
        </div>
        <div class="social">
            <h3>
                Acompanhe nossas redes sociais
            </h3>
            <ul>
                <li><a href="#">Instagram</a></li>
                <li><a href="#">Twitter</a></li>
                <li><a href="#">Facebook</a></li>
                <li><a href="#">Youtube</a></li>
            </ul>
        </div>
        <div class="cadastro_email">
            <h3>
                Cadastre seu e-mail para receber novidades
            </h3>
            <input type="text" placeholder="E-MAIL">
            <button>OK</button>
        </div>
    </footer>
</template>

<script>

</script>

<style scoped>
footer {
    background-color: rgb(167, 133, 106);
    align-items: center;
    justify-content: center;
}

div {
    margin: 40px;
}

h2 {
    margin: 5px;
}

img {
    width: 60px;
    height: 60px;
}

ul {
    list-style: none;
}

li {
    margin: 5px;
}

a {
    text-decoration: none;
    color: rgb(236, 228, 218);
    margin: 5px;
}

a:hover {
    color: rgb(61, 61, 61);
}

.cadastro_email input {
    width: 250px;
    height: 30px;
}

.cadastro_email button {
    width: 125px;
    height: 33px
}

</style>