<template>
  <div id="app">
    <MtG />
  </div>
</template>

<script>
import MtG from './components/MtG.vue'

export default {
  name: 'app',
  components: {
    MtG
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  width: 100%;
  height: 100vh;
  background-color: grey;
  padding-top: 100px;
}
</style>
