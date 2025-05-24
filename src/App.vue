<!-- src/App.vue -->
<template>
  <div class="bg-gray-100 min-h-screen">
    <NavBar />
    <main class="pt-20">
      <Hero />
      <About />
      <Projandexp />
    </main>
  </div>
</template>

<script setup lang="ts">
import NavBar     from './components/NavBar.vue'
import Hero       from './components/Hero.vue'
import About      from './components/About.vue'
import Projandexp from './components/Projandexp.vue'
</script>


