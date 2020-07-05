<template>
  <div class="hello">
     <form method="get" action=".">
        <input v-model="name" placeholder="name" name="name" type="text" id="name" value="" size="10" maxlength="9" />
        <input v-model="email" placeholder="email" name="email" type="email" id="email" size="60" />
        <input v-model="telefone" placeholder="telefone" name="telefone" type="tel" id="telefone" size="40" />
        <input v-model="cpf" placeholder="cpf" name="cpf" type="tel" id="cpf" size="40" />
      </form>
      {{'nome:' + name}}
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
  </div>
</template>

<script>
export default {
  name: 'index',
  data () {
    return {
      msg: 'Teste Full Stack Qualicor',
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
</style>
