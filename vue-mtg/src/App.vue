<template>
  <div id="app">
    <MtGcard
      cardName="遅刻許可"
      pictureSrc="https://pbs.twimg.com/profile_images/719895139146031104/XgAKgZvu_400x400.jpg"
      type="インスタント"
      expansion="scouty"
      cardText="記事1つを対象とし、その締切を1日伸ばす。"
    />
    <div style="margin-left: 10px;">
      <img src="http://gatherer.wizards.com/Handlers/Image.ashx?multiverseid=442288&type=card" />
    </div>
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
