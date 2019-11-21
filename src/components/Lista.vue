<template>
 <div>
   <div v-bind:key="elemento.id" v-for="elemento in lista">
     <ListaElemento v-bind:elemento="elemento"/>
   </div>
 </div>
</template>

<script>
import ListaElemento from './ListaElemento';


export default{
  name: "Lista",
  components:{
    ListaElemento
  },
  props : ["lista"]
}

</script>

<style scoped>

</style>