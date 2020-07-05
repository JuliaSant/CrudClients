<template>
  <div class="hello">
     <form method="get" action=".">
        <input v-model="name" class="formInput" placeholder="name" name="name" type="text" id="name" value="" size="10" maxlength="9" />
        <input v-model="email" class="formInput" placeholder="email" name="email" type="email" id="email" size="60" />
        <input v-model="telefone" class="formInput" placeholder="telefone" name="telefone" type="tel" id="telefone" size="40" />
        <input v-model="cpf" class="formInput" placeholder="cpf" name="cpf" type="tel" id="cpf" size="40" />
        <button @submit="aa" class="btn btn-success">Cadastrar</button>
      </form>
      {{'nome:' + name}}
  </div>
</template>

<script>
export default {
  name: 'index',
  data () {
    return {
      name: '',
      email: '',
      cpf: '',
      telefone: ''
    }
  }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.formInput {
  width: 50%;
  padding: 1em;
  margin: .2em;
  border: none;
  background-color: antiquewhite;
  border-radius: 1em;
}
.formInput:focus {
  outline: 0;
}
.btn-success  {
  width: 30%;
  margin: .4em;
  padding: 1em;
}
</style>
