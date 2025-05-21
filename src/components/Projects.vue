<template>
  <section id="projects" class="py-20 bg-white">
    <h2 class="text-4xl font-semibold text-center mb-8">Projects</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      <!-- Example card -->
      <div class="p-4 border rounded-lg shadow">
        <h3 class="text-2xl font-medium">Portfolio Website</h3>
        <p class="mt-2 text-sm">Built with Vue 3, TypeScript &amp; Tailwind.</p>
        <a href="https://github.com/Ryo0326-hub/ryoswebsite" class="text-blue-600 mt-2 inline-block">
          View on GitHub →
        </a>
      </div>
      <!-- repeat for each project -->
    </div>
  </section>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({ name: 'Projects' })
</script>
