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
      <div class="parallelogram-container mb-4">
        <img
          src="../assets/ryo2.jpg"
          alt="Ryo's Photo"
          class="w-full h-full object-cover"
        />
      </div>
      <div class="max-w-3xl text-lg leading-relaxed text-center space-y-4">
        <p>
          Hi, I’m Ryo Kitano, a second-year math student at the University of Waterloo majoring in
          Mathematical Finance and Combinatorics & Optimization. I'm passionate about applying technical and analytical
          skills in software development and quantitative research.
        </p>

        <p>
          My love for numbers actually began much earlier than university. In 3rd grade,
          I spent hours every day playing Pokemon on my 3DS. From these games, I learned to strategize by optimizing team compositions, analyzing the probability for
          shiny pokemons, and beating opponents in battles. I think my game addiction during childhood has unknowingly ingrained my passion for mathematics.
        </p>

        <p>
          When I'm not building financial models, you'll find me watching NBA games. Basketball fascinates me because there are numbers everywhere. 
          I love the mathematical beauty in analyzing player performance and team mechanics. 
        </p>

        <p>
          Above all, I aspire to become a quant. I want to unveil the hidden patterns in financial data that are seamingly impossible to see. 
          I will continuously challenge myself both academically and as a person while being excited for what the future holds for me and the world.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
// No logic needed for this static section
</script>

<style scoped>
.parallelogram-container {
  width: 250px;
  height: 250px;
  position: relative;
  overflow: hidden;
  transform: skew(-5deg); /* Further reduced skew angle from -10deg to -5deg */
  display: inline-block;
  box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
}

.parallelogram-container img {
  transform: skew(5deg) scale(1.15); /* Added scale(1.15) to zoom in by 15% */
  position: relative;
  left: -5px; /* Reduced offset from -10px to -5px */
  width: calc(100% + 10px); /* Adjusted width calculation */
  object-position: center; /* Center the image focus */
}
</style>
