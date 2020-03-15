<template>
  <div id="app">
    <head-nav/>
    <section1/>
    <div style="clear:both"></div>
    <foot/>
  </div>
</template>

<script>
import HeadNav from './components/HeadNav.vue'
import Section1 from './components/Section.vue'
import Foot from './components/Foot.vue'
export default {
  name: 'App',
  components: {
    HeadNav,
    Section1,
    Foot
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 0;
  padding: 0;
}
</style>
