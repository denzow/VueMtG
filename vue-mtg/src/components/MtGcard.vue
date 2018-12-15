<template>
  <div class="mtg">
    <div class="card-base">
      <div class="card-background">
        <div class="card-inner">
          <div class="card-header">
            <span>{{ cardName }}</span>
            <span>
              <span class="mana fas fa-tint"></span>
              <span class="mana fas fa-tint"></span>
            </span>
          </div>
          <div class="card-picture-base">
            <img class="card-picture" :src="pictureSrc">
          </div>
          <div class="card-category">
            <span>{{ type }}</span>
            <span>{{ expansion }}</span>
          </div>
          <div class="card-text-container">
            <div class="card-text">
              {{ cardText }}
            </div>
          </div>
        </div>
      </div>
    </div>
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.6.1/css/all.css" integrity="sha384-gfdkjb5BdAXd+lj+gudLWI+BXq4IuLW5IT+brZEZsLFm++aCMlF1V92rMkPaX4PP" crossorigin="anonymous">
  </div>
</template>

<script>
export default {
  name: 'MtG',
  props: {
    cardName: {
      type: String,
      default: '',
    },
    pictureSrc: {
      type: String,
      default: '',
    },
    type: {
      type: String,
      default: '',
    },
    expansion: {
      type: String,
      default: '',
    },
    cardText: {
      type: String,
      default: '',
    },
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
  padding: 5px 2px 5px;
  height: 260px;
}
.card-inner {
  width: 100%;
  display: flex;
  flex-direction: column;
}


.mana {
  margin: 1px;
  width: 8px;
  padding: 1px;
  border-radius: 6px;
  background-color: #8eb9ff;
  box-shadow: -1px 1px 1px 1px rgba(0,0,0,0.8);
}


.card-category,
.card-header {
  height: 12px;
  background-color: #AACCFF;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 8px;
  font-weight: 700;
  padding: 2px;
  border: 2px ridge #22AADD;
  border-radius: 5px;
}

.card-picture-base {
  height: 140px;
  background-color: black;
  margin: 0 3px;
  border-width: 0 2px;
  border-style: ridge;
  border-color: #22AADD;
}

.card-picture {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.card-text-container {
  height: 92px;
  background-color: #EEEEFF;
  margin: 0 3px;
  font-size: 9px;
  display: table;
  border-width: 0 2px 2px;
  border-style: ridge;
  border-color: #22AADD;

  .card-text {
    display: table-cell;
    vertical-align: middle;
  }
}
</style>
