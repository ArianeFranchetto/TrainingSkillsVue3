<template>
<div>
  <h3>Training skills</h3>
    <DiretivasOne/>
    <MetodosOne/>
  </div>
</template>

<script>
import DiretivasOne from './components/DiretivasOne.vue';
import MetodosOne from './components/MetodosOne.vue';

export default {
  name: 'App',
  components: {
    DiretivasOne,
    MetodosOne,
  }
}
</script>

<style>
* {
  background-color: burlywood;
}

</style>
