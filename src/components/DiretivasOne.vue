<template>
    <span>V-MODEL</span>
<h2 :v-model="nome">{{ nome }}</h2>

    <span>V-IF</span>
<h2 v-if="conteudo">mostrando</h2>
<h2 v-else>oculto</h2>

<h2 v-if="1 == 2">2</h2>
<h2 v-else>erro</h2>

</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent ({
name: "DiretivasOne",


 data () {
    return {
        nome: 'ariane',
        conteudo: true,
    }
 }
})

</script>