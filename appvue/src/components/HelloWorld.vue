<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div>
      <span v-if="visibilidade">Olá estou aprendendo Vue.JS</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    visibilidade: Boolean 
  },/* ,
  data: {
    visibilidade: false
  } */
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>
