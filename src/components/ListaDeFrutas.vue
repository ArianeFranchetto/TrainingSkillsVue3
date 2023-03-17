<template>
<div class="lista">
    <h3>Lista de Frutas</h3>

    <h5>V-FOR E USAR METHODS PARA MUDAR O ESTADO</h5>
    <input v-model="novaFruta">

    <button @click="inserirFruta">Inserir</button><br>
    <span>Lista de Frutas</span><br>
    <ul>
        <li v-for="fruta in frutas">{{ fruta }}</li>
    </ul>
    <span>Total: <b>{{ totalFrutas }}</b></span>

</div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent ({
    name: 'ListaDeFrutas',

    data () {
        return {
            frutas: [],
            novaFruta: '',
            totalFrutas: 0

        }
    },
    methods: {
        inserirFruta () {
            this.frutas.push(this.novaFruta)
            this.novaFruta = ''
            this.totalFrutas = this.frutas.length
        }
    }
})
</script>

<style>
.lista {
    background-color: chocolate;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    border-radius: 20px;
}

ul {
    list-style: none;
    
}

</style>