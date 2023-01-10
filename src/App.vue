<template>
 <div id="app" class="container">
   <div class="row">
     <div class="col-md-12">
       <h1>LISTADO CLIENTES</h1>
     </div>
   </div>
   <div class="row">
     <div class="col-md-12">
       <TablaClientes />
     </div>
   </div>
 </div>
</template>

<script>
import TablaClientes from "@/components/TablaClientes.vue";

export default {
  name: 'App',
  components: {
    TablaClientes,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
