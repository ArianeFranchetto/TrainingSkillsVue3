<template>
    <span>V-MODEL</span>
<h2 :v-model="nome">{{ nome }}</h2>

    <span>V-IF</span>
<h2 v-if="conteudo">mostrando</h2>
<h2 v-else>oculto</h2>

<h2 v-if="1 == 2">2</h2>
<h2 v-else>erro</h2>

<span>V-FOR (ciclo)
    interação, percorrer vários elementos, ex: percorrer uma lista
sempre nome em nomes/ igredientes em igredientes
</span>

<p v-for="ingrediente in ingredientes">
    {{ ingrediente }}

</p>

<p v-for="pessoa in pessoas">
    {{ pessoa.nome }}
    {{ pessoa.idade }}

</p>

</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent ({
name: "DiretivasOne",


 data () {
    return {
        nome: 'ariane',
        conteudo: true,
        ingredientes: [
            "alface",
            "presunto",
            "queijo"
        ],

        pessoas: [
            {nome:"ariane", idade: 26},
            {nome: "caio", idade: 29}
        ]

    }
 }
})

</script>