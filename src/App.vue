<template>
  <div id="app">
    <AvadaHeader/>
    <AvadaMain/>
    <AvadaFooter/>
  </div>
</template>

<script>
import AvadaHeader from './components/AvadaHeader.vue'
import AvadaMain from './components/AvadaMain.vue'
import AvadaFooter from './components/AvadaFooter.vue'

export default {
  name: 'App',
  components: {
    AvadaHeader, AvadaMain, AvadaFooter
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
