<template>
  <div id="app">
      <Lista v-bind:lista="lista"/>
  </div>
</template>

<script>
import Lista from './components/Lista';

export default {
  name: 'app',
  components: {
      Lista
  },
  data() {
    return {
      lista:[
        {
          id:1,
          titulo: "Hacer uno",
          completed: false
        },
        {
          id:2,
          titulo: "Hacer dos",
          completed: true
        },
        {
          id:3,
          titulo: "Hacer tres",
          completed: false
        }
      ]
    }
  }
}
</script>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body{
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}

</style>
