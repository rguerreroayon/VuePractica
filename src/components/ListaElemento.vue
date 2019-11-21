<template>
    <div class="lista-elemento" 
         v-bind:class="{'is-complete':elemento.completed}"> 
        <p>{{elemento.titulo}}</p>
    </div>
</template>


<script >
export default {
    name:"ListaElemento",
    props:["elemento"]
}
</script>

<style scoped>
    .lista-elemento{
        background: #f4f4f4;
        padding: 10px;
        border-bottom:1px #ccc dotted;
    }

    .is-complete{
        text-decoration: line-through;
    }

    .del{
        background-attachment: #ff0000;
        color: #fff;
        border: none;
        padding: 5px 9px;
        border-radius: 50%;
        cursor: pointer;
        float: right;
    }
</style>