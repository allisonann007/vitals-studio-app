<!--Incorporate data from an API-->
<template>
<div>
  <p v-if="$fetchState.pending">Fetching API...</p>
  <p v-else-if="$fetchState.error">An error occurred</p>
  <div v-else>
    <h1>Cart</h1>
    <!--Build a corresponding component and use v-for to loop over the data-->
    <ul>
      <li v-for="mountain of mountains">{{ mountain.title }}</li>
      <li v-for="mountain of mountains">{{ mountain.continent }}</li>
      <li v-for="mountain of mountains">{{ mountain.height }}</li>
      <li v-for="mountain of mountains">{{ mountain.countries }}</li>
    </ul>
    <!--The component should have some sort of method that causes a UI interaction on that instance of the component-->
    <!--Click first button, then hit refresh and text appears by way of built-in Vue Transition component-->
    <button @click="show = !show">UI Interaction button</button>
    <Transition>
      <p v-if="show">This button has been clicked!</p>
    </Transition>
    <button @click="$fetch">Refresh</button>
  </div>
</div>
</template>

<!--That component should have props validation as well as use at least 4 data points
in the template itself (heading, description, image, statistics, etc).-->
<script>
export default {
  data() {
    return {
      mountains: []
    }
  },
  async fetch() {
    this.mountains = await fetch(
      'https://api.nuxtjs.dev/mountains'
    ).then(res => res.json())
  }
}
</script>

<!--The component should have some sort of method that causes a UI interaction on that instance of the component-->
<style>
.v-enter-active,
.v-leave-active {
  transition: opacity 3s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
