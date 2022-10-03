<template>

<div id="app">
  <!--  <img  v-bind:key="item" :src="require('../assets/' + item + '.jpg')" width="500">-->
  <ImageMarkup :title="item.title" :alt="item.alt" :src="item.src" v-for="(item,id) in images" :key="id" />
</div>
</template>
<!--The image component should have props for at least the image src, alt, & title attributes, use prop validation.-->
<!--Refactored into component props and validation-->
<script>
import ImageMarkup from './ImageMarkup.vue';

export default {
  components: {
    ImageMarkup
  },
  data() {
    return {
      images: [{
          title: 'processOne',
          alt: 'two women blowing glass with furnace',
          src: '/assets/processOne.jpg'
        },
        {
          title: 'processTwo',
          alt: 'woman blowing glass',
          src: '/assets/processTwo.jpg'
        },
        {
          title: 'processThree',
          alt: 'two woman blowing glass at bench',
          src: '/assets/processThree.jpg'
        }]
    }
  },
  // Within your pages, add the head method to the script and include
  // the hid meta line to overwrite the description on a page by page basis
  head() {
    return {
      meta: [
        {hid: 'description', name: 'description', content: 'Process Page meta data'},
      ]
    }
  }
}
</script>
