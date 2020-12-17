<template>
  <div id="app">
    <p> Je voulais utiliser la fonction random() 
      en scss pour afficher les cercle aléatoirement, 
      cependant j'ai eu un probleem en essayant d'installer 
      SCSS ce qui a générer plein de bug et m'a fait perdre tout mon temps...</p>
    <HelloWorld msg="test Delia solution"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
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
