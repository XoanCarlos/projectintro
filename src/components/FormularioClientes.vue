<template>
  <div id="formulario-clientes">
    <form>
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <label>Nombre: </label>
            <input type="text" class="form-control" />
          </div>
          <div class="col-md-4">
            <label>Apellidos: </label>
            <input type="text" class="form-control" />
          </div>
          <div class="col-md-4">
            <label>email: </label>
            <input type="text" class="form-control" />
          </div>
        </div>
        <div class="row">
          <div class="row-cols-md-4">
            <div class="form-group">
              <br/>
            <button class="btn btn-primary">Guardar</button>
            </div>
          </div>
        </div>
      </div>
    </form>

  </div>

</template>

<script>
export default {
  name: "FormularioClientes",
  data(){
    return{
      cliente: {
        nombre: '',
        apellidos: '',
        email: '',
      }
    }
  }
}
</script>

<style scoped>
  form {
    margin-bottom: 2rem;
  }
</style>