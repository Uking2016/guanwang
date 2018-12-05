<template>
  <div id="app">
    <index/>
  </div>
</template>

<script>
import Vue from 'vue'
import index from './components/index.vue'
import VueLazyLoad from 'vue-lazyload'
Vue.use(VueLazyLoad, {
  preLoad: 1
})
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
