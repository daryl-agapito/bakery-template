<script setup>
import Hero from '../components/homepage/Hero.vue'
import Navbar from '../layouts/globals/Navbar.vue'
import ProductsHighlight from '../layouts/globals/ProductsHighlight.vue'
import Reviews from '../components/homepage/Reviews.vue'
import Services from '../components/homepage/Services.vue'
import Test from '../components/homepage/Test.vue'
</script>

<template>
  <main>
    <Navbar />
    <Hero />
    <ProductsHighlight />
    <Reviews />
    <Services />
    <Test />
  </main>
</template>
