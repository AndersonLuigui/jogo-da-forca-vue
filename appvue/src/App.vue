<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Olá mundo!"/>
    <NovoComponente texto="A diretiva v-text permite a apresentação
    de textos, tal como ocorre quando usamos diretivas diretas"/>
    <terceiroComponente texto="Olá Vue hahahah"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NovoComponente from'./components/NovoComponente.vue'
import terceiroComponente from'./components/terceiroComponente.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    NovoComponente,
    terceiroComponente
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
