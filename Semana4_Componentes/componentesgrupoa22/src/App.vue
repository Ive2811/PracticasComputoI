<template>
  <div id="app">
    <header-title title="Programacion Computacional IV"/>
    <product-list/>
  </div>
</template>

<script>

import HeaderTitle from './components/HeaderTitle'
import ProductList from './components/ProductList.vue'

export default {
  name: 'App',
  components: {
    HeaderTitle,
    ProductList
    
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
