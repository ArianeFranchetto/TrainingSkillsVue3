<template>
<div>
  <h3>Training skills</h3>
    <DiretivasOne/>
    <MetodosOne/>
    <ListaDeFrutas/>
    <MudarGato/>
   
  </div>
</template>

<script>
import DiretivasOne from './components/DiretivasOne.vue';
import MetodosOne from './components/MetodosOne.vue';
import ListaDeFrutas from './components/ListaDeFrutas.vue';
import MudarGato from './components/MudarGato.vue';


export default {
  name: 'App',
  components: {
    DiretivasOne,
    MetodosOne,
    ListaDeFrutas,
    MudarGato,
    
  }
}
</script>

<style>
* {
  background-color: burlywood;
}

</style>
