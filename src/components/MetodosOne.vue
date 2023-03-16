
<template>
    <span>
        MÉTODOS
    </span>

    <div v-if="visivel">
        DIV1
    </div>
    <div v-else>
        DIV2
    </div>
<button @click="mostrarEsconder">
click
</button>



</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent
    ({
        name: 'MetodosOne',

        data () {
            return {
                visivel: true 
            }
           
        },

        methods: {
                mostrarEsconder () {
                    this.visivel = !this.visivel

                },

                }

            }
        

    )
</script>