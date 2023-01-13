<template>
 <div id="app" class="container">
   <div class="row">
     <div class="col-md-12">
       <h1>LISTADO CLIENTES</h1>
     </div>
   </div>
   <div class="row">
     <div class="col-md-12">
       <formulario-clientes />
       <tabla-clientes :clientes = 'clientes' />
     </div>
   </div>
 </div>
</template>

<script>
import TablaClientes from "@/components/TablaClientes.vue";
import FormularioClientes from "@/components/FormularioClientes.vue";

export default {
  name: 'App',
  components: {
    FormularioClientes,
    TablaClientes,
  },
  data(){
    return{
       clientes:[
         {
         id: 1,
         nombre: 'Lou',
         apellidos: 'Reed',
         email: 'lreed@mail.com',
         },
        {
          id: 2,
          nombre: 'Carlos',
          apellidos: 'Santana',
          email: 'csantana@mail.com',
        },
        {
          id: 3,
          nombre: 'Janis',
          apellidos: 'Joplin',
          email: 'jjoplin@mail.com',
        },
         {
           id: 4,
           nombre: 'Bruce',
           apellidos: 'Springteen',
           email: 'bruce@mail.com',
         },
       ],
      }
     },
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
