<template>
  <div class="mtg">
    <div class="card-base">
      <div class="card-background">
        <div class="card-inner">
          <div class="card-header">
            <span>対抗呪文</span>
            <span>青青</span>
          </div>
          <div class="card-picture">
          </div>
          <div class="card-category">
            <span>インスタント</span>
            <span>scouty</span>
          </div>
          <div class="card-text-container">
            <div class="card-text">
              呪文１つを対象とし、それを打ち消す。
            </div>
          </div>
        </div>
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
  height: 280px;
  border-width: 10px 10px 20px;
  border-color: #000;
  border-style: solid;
  border-radius: 15px;
  background-color: #000;
}

.card-background {
  border-radius: 4px 4px 15px 15px;
  background-color: #00AAFF;
  padding: 5px 5px 5px;
  height: 260px;
}
.card-inner {
  height: 275px;
  width: 100%;
  display: flex;
  flex-direction: column;
}

.card-category,
.card-header {
  height: 13px;
  background-color: #AACCFF;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 8px;
  padding: 2px;
}

.card-picture {
  height: 142px;
  background-color: black;
}

.card-text-container {
  height: 100px;
  background-color: #EEEEFF;
  font-size: 9px;
  display: table;

  .card-text {
    display: table-cell;
    vertical-align: middle;
  }
}
</style>
