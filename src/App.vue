<template>
  <div id="app">
    <LavaLamp msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import LavaLamp from './components/LavaLamp.vue'

export default {
  name: 'App',
  components: {
    LavaLamp
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Montserrat', sans-serif;
}

body {
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -webkit-tap-highlight-color: transparent;
}

#app {
  height: 100vh;
  width: 100vw;
  overflow: hidden;
  position: fixed;
}
</style>
