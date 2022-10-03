<template>
<div id="app">
<h1> {{ heading }}</h1>
<img src="./../assets/about-img.png" width="600">
</div>
</template>

<!--All repeated content is from variables in the <script> section of the .vue file.-->
<script>

export default {
name: 'app',
data () {
return {
heading: 'Celebrating glassmaking at its source.'
}
},
// Within your pages, add the head method to the script and include
// the hid meta line to overwrite the description on a page by page basis
head() {
  return {
    meta: [
      {hid: 'description', name: 'description', content: 'About Page meta data'},
    ]
  }
}
}

</script>
