<template>
  <div id="app">
    <index/>
  </div>
</template>

<script>
import index from './components/index.vue'

export default {
  name: 'app',
  components: {
    index
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
html,body{
  padding: 0;
  margin: 0;
}
</style>
