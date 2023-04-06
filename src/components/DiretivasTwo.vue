
<template>
    <div>
        <h3>V-HTML</h3>
        <span>O v-html é usado para que o JS interaja diretamente com o DOM
            sendo assim é usado html dentro do JS e interpretado no código como HTML

            <span v-html="valor"></span>

            <button @click="t1">Title</button>
            <button @click="t2">Title</button>
            <button @click="t3">Title</button>

        </span>
    </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent
    ({
        name: 'DiretivasTwo',

        data() {
            return {
                valor: '<h1>Testando o v-html</h1>'
            }
},

methods: {
        t1() {
            this.valor = '<h5>title novo</h5>'
        },
        t2() {
            this.valor = '<input type=text>insira</input>'
        },
        t3() {
            this.valor = '<h2>title novo</h2>'
        }

    }


  }  )
</script>