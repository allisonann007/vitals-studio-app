<template>
<div>
  <nav>
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="/AboutPage">About</NuxtLink>
    <NuxtLink to="/DiscoverPage">Discover</NuxtLink>
    <NuxtLink to="/ProcessPage">Process</NuxtLink>
    <NuxtLink to="/ShopPage">Shop</NuxtLink>
    <NuxtLink to="/CartPage">Cart</NuxtLink>
    <NuxtLink to="/childPage">Child Page</NuxtLink>
  </nav>
  <Nuxt />
</div>
</template>

<style>
* {
  font-family: 'Quicksand', sans-serif;
}
nav {
  font-size: 5vw;
}
</style>
