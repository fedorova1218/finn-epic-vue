<template>
  <div class ='v-carusel-item'>
      <img class="card" :src= "require ('../assets/' + item_data.img)" alt = "">
  </div>
</template>

<script>

export default{
  name: 'v-carusel-item',
  props: {
      item_data: {
        type: Object,
        default: () => {}
      }
  },
  data() {
    return {}
  },

  computed: {}
}
</script>

<style lang = "scss">
.card{
  width: 260px;
  height: 446px;
  filter: drop-shadow(8px 8px 15px rgba(0, 0, 0, 0.25));
  border-radius: 20px;
  margin: 7vh;
}

.card:hover {
  -webkit-transform: translateX(-10px);
  transform: translateY(-10px);
  animation-duration: 20s;
  animation-timing-function:ease-in-out;

}
</style>