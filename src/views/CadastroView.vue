<template lang="">
    <main>
        <div>
            <br> <br>
            <h1>Indique seu Botequim favorito!</h1> <br>
            <h2>Regras para a indicação:</h2> <br> <br>
            <ol>
                <li>O buteco deve ser familiar: o dono ou a família deve estar à frente, trabalhando no negócio.</li> <br>
                <li>O buteco não pode pertencer a rede ou ser uma franquia</li>
            </ol> <br><br>
            <h2>Preencha os dados do estabelecimento nos campos abaixo:</h2> <br> <br>
        </div>
        <form>
            <input type="text" placeholder="Nome do Botequim">
            <input type="text" placeholder="Endereço">
            <textarea id="botequim_do_coracao" cols="30" rows="10" placeholder="Por que esse é seu botequim de coração?"></textarea>
            <input type="text" placeholder="Redes Sociais">
            <input type="text" placeholder="Telefone">
            <input type="text" placeholder="Email">
            <button type="submit">Enviar</button>
        </form>
    </main>
</template>
<script>
export default {
    
}
</script>
<style scoped>
form {
    display: flex;
    flex-direction: column;
    width: 50%;
    margin: auto;
    margin-bottom: 35px;
}

input {
    margin-top: 15px;
    height: 35px;
}

textarea{
    margin-top: 15px;
    font-family: Avenir, Helvetica, Arial, sans-serif;
}

button {
    margin-top: 15px;
    height: 35px;
    width: 50%;
    transform: translate(50%);
}

</style>