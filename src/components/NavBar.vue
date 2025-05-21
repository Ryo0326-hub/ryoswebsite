<!-- src/components/NavBar.vue -->
<template>
  <nav class="fixed w-full bg-white shadow z-10">
    <ul class="container mx-auto flex justify-end space-x-6 p-4">
      <li><a href="#hero"    class="hover:text-blue-600">Home</a></li>
      <li><a href="#about"   class="hover:text-blue-600">About</a></li>
      <li><a href="#projects"class="hover:text-blue-600">Projects</a></li>
      <li><a href="#experience" class="hover:text-blue-600">Experience</a></li>
      <li><a href="#contact" class="hover:text-blue-600">Contact</a></li>
    </ul>
  </nav>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({ name: 'NavBar' })
</script>
