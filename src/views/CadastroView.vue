<template>
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
        <FormComponent />
    </main>

</template>
<script setup>
import { ref } from 'vue'

const count = ref(0)

import FormComponent from "@/components/FormComponent.vue"

</script>
<style scoped>
</style>