<template>
  <div class="mtg">
    <div class="card-base">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style lang="scss" scoped>
.mtg {
  display: flex;
  justify-content: center;
}

.card-base {
  width: 220px;
  height: 310px;
  border: solid 10px #000;
  border-radius: 15px;
}
</style>
