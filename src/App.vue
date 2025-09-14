<script setup lang="ts">
import Header from './components/Header/Header.vue';
import ProductSection from './components/ProductSection/ProductSection.vue';
import BoseCategory from './components/BoseCategory/BoseCategory.vue'
</script>

<template>
  <div>
  <Header/>
  <ProductSection/>
  <BoseCategory/>

  </div>
</template>



<style>
html {
  scroll-behavior: smooth;
}
body {
  margin: 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
img {
  width: 100%;
}
</style>


