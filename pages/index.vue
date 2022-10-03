<!--Converted to Nuxt framework-->
<!--Your site should have at least 4 pages (including the home) with <nuxt-link> used to navigate between them-->
<!--Added routing for all pages using pages directory and <nuxt-link>-->
<!--Created all 4 required pages-->
<template>
<div id="app">
<h1> {{ welcome }}</h1>
<img src="./../assets/home-img.jpg" width="600">
</div>
</template>

<script>
export default {
name: 'app',
data () {
return {
welcome: 'Connect to the healing truth of creativity.  Discover original stories.'
}
}
}
</script>

<style>
#app {
  color: #000000;
  text-align: center;

}
@keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
    -webkit-animation: fadein 5s;
}
</style>
