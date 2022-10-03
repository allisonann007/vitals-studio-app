<template>
<div id="app">
  <h1>{{ message }}</h1>
  <!-- A v-if and v-else is used to change content of UI -->
  <div v-if="seen">
    <img src="./../assets/shop-piece.jpeg" width="200" alt="yellow and jade green vase">
    <img src="./../assets/shop-piece-2.png" width="200" alt="black and yellow vase">
    <img src="./../assets/shop-piece-3.jpeg" width="150" alt="magenta, amber and jade green vase">
    <img src="./../assets/shop-sandwich.jpeg" width="200" alt="glass cheeseburger sculpture">
  </div>
  <h1 v-else>Shop page under construction.</h1>

</div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      seen: true,
      message: 'Shop'
    }
  },
  // Within your pages, add the head method to the script and include
  // the hid meta line to overwrite the description on a page by page basis
  head() {
    return {
      meta: [
        {hid: 'description', name: 'description', content: 'Shop Page meta data'},
      ]
    }
  }
}
</script>

<style lang="scss">



</style>
