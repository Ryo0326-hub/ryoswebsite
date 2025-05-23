<template>
  <section id="about" class="py-16 bg-gray-100 relative">
    <!-- About Me Title with Icon -->
    <div class="section-header mb-1/2">
      <img 
        src="../assets/infinity.png" 
        alt="Infinity Symbol" 
        class="icon-pulse" 
      />
      <h2>About Me</h2>
    </div>
    <!-- Photo and Main Description -->
    <div class="max-w-4xl mx-auto flex flex-col items-center">
      <img
        src="../assets/ryo.jpg"
        alt="Ryo's Photo"
        class="w-1/4 h-1/4 rounded-full shadow-lg object-cover mb-4"
      />
      <p class="max-w-2xl text-lg leading-relaxed text-center">
        Hi, I’m Ryo Kitano, a second-year math student at the University of Waterloo. I specialize in
        Mathematical Finance and Combinatorics & Optimization, where I explore technical and analytical 
        applications in software development and quantitative research.
      </p>
    </div>
  </section>
</template>

<script setup lang="ts">
// No logic needed for this static section
</script>
