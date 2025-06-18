<template>
  <section id="about" class="py-8 md:py-16 relative about-bg">
    <!-- About Me Title with Icon -->
    <div class="section-header mb-4 md:mb-8">
      <h2>About Me</h2>
    </div>
    <!-- Photo and Main Description -->
    <div class="max-w-4xl mx-auto flex flex-col items-center px-4">
      <div class="max-w-3xl text-base md:text-lg leading-relaxed text-center space-y-3 md:space-y-4">
        <p>
          Hi, I'm Ryo Kitano, a second-year math student at the University of Waterloo majoring in
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
.about-bg {
  position: relative;
  min-height: 400px;
  background: #fff;
}

/* Mobile-first parallelogram container */
.parallelogram-container {
  width: 200px; /* Smaller on mobile */
  height: 200px;
  position: relative;
  overflow: hidden;
  transform: skew(-3deg); /* Less skew on mobile for better visibility */
  display: inline-block;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15); /* Lighter shadow on mobile */
}

.parallelogram-container img {
  transform: skew(3deg) scale(1.1); /* Less skew and scale on mobile */
  position: relative;
  left: -3px; /* Smaller offset */
  width: calc(100% + 6px); /* Adjusted width calculation */
  object-position: center;
}

/* Desktop parallelogram styles */
@media (min-width: 768px) {
  .parallelogram-container {
    width: 250px; /* Desktop size */
    height: 250px;
    transform: skew(-5deg); /* Desktop skew */
    box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2); /* Desktop shadow */
  }

  .parallelogram-container img {
    transform: skew(5deg) scale(1.15); /* Desktop transform */
    left: -5px; /* Desktop offset */
    width: calc(100% + 10px); /* Desktop width */
  }
}
</style>
