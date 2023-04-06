
<template>
    <div>
        <h2>v-once significa uma vez, que é a primeira vez, todo conteudo de um elemento
            seja apresentado mas nao seja modificado

            e v-pre (antes) todo código que estiver no ve pré vai ser apresentado antes
            do resto do cód
        </h2>
        <p v-pre></p>
        <p v-once>{{ nome }}</p>
        <p v-text="nome"></p>
        <button @click="executar">Click</button>



    </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent
    ({
        name: 'DiretivasThree',

        data() {
            return {
                nome: "João"

            }
        },

        methods: {
            executar() {
                this.nome = "Antonio"

            }


        }


    })
</script>