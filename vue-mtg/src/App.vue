<template>
  <div id="app">
    <MtGcard />
    <div style="margin-left: 10px;">
      <img src="http://gatherer.wizards.com/Handlers/Image.ashx?multiverseid=442288&type=card" />
    </div>
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.6.1/css/all.css" integrity="sha384-gfdkjb5BdAXd+lj+gudLWI+BXq4IuLW5IT+brZEZsLFm++aCMlF1V92rMkPaX4PP" crossorigin="anonymous">
  </div>
</template>

<script>
import MtGcard from './components/MtGcard.vue'

export default {
  name: 'app',
  components: {
    MtGcard
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
  display: flex;
  justify-content: center;
}
</style>
