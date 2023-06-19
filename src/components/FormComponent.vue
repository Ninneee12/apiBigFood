<template>
    <form>
        <input type="text" placeholder="Nome do Botequim">
        <input type="text" placeholder="Endereço">
        <textarea id="botequim_do_coracao" cols="30" rows="10" placeholder="Por que esse é seu botequim de coração?"></textarea>
        <input type="text" placeholder="Redes Sociais">
        <input type="text" placeholder="Telefone">
        <input type="text" placeholder="Email">
        <button type="submit">Enviar</button>
    </form>
</template>

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