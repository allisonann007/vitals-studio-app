<template>
<nav>
  <!--Converted to Nuxt framework-->
  <!--Your site should have at least 4 pages (including the home) with <nuxt-link> used to navigate between them-->
  <!--Added routing for all pages using pages directory and <nuxt-link>-->
  <!--Created all 4 required pages-->
  <NuxtLink to="/">Home</NuxtLink>
  <NuxtLink to="/AboutPage">About</NuxtLink>
  <NuxtLink to="/DiscoverPage">Discover</NuxtLink>
  <NuxtLink to="/ProcessPage">Process</NuxtLink>
  <NuxtLink to="/ShopPage">Shop</NuxtLink>
  <NuxtLink to="/CartPage">Cart</NuxtLink>
</nav>
</template>

<script>
export default {
  name: 'app',
}
</script>

<style>
#app {
  font-weight: lighter;
  color: #000000;
  text-align: center;
  font-style: 'Montserrat', sans-serif;
  text-decoration: none;
}
</style>
