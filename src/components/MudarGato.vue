<template>
    <div class="geralzinho">
        <h3>V-BIND (ligar) E V-ON</h3>
        <h4>O gatinho selecionado é {{ gato }}</h4>
        <img v-bind:src="imagem">
        <button @click="mostrarGatoComendo">Gato comendo</button>
        <button @click="mostrarGatoRindo">Gato rindo</button>

    </div>

</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent ({
    nome: 'MudarGato',

    data () {
        return {
            gato:'',
            imagem: ''
            
        }
    },
    methods: {
        mostrarGatoComendo () {
            this.gato = 'GatoComendo'
            this.imagem = '/img/gato-peixe.png'
        },

        mostrarGatoRindo () {
            this.gato = 'GatoRindo',
            this.imagem = '/img/gato-rindo.png'
        }
       
            
        }

    }
)


</script>

<style>
.geralzinho {
    background-color: darkgreen;
}

img {
    width: 100px;
    height: 100px;
    border-radius: 50px;
}

</style>