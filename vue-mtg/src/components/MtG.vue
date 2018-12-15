<template>
  <div class="mtg">
    <div class="card-base">
      <div class="card-inner">

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MtG',
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
  width: 203px;
  height: 271px;
  border: solid 10px #000;
  border-radius: 15px;
  background-color: #5599EE;
  padding: 5px 5px 15px;
}

.card-inner {
  background-color: red;
  height: 100%;
  width: 100%;
}
</style>
