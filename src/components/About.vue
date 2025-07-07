<template>
  <section id="about" class="py-4 md:py-8 relative about-bg">
    <!-- About Me Title with Icon -->
    <div class="section-header mb-1 md:mb-2">
      <h2>About Me</h2>
    </div>
    <!-- Photo and Main Description -->
    <div class="max-w-4xl mx-auto flex flex-col items-center px-4">
      <div class="max-w-3xl text-base md:text-lg leading-relaxed text-center space-y-3 md:space-y-4">
        <p>
          I'm Ryo, a second year mathematics student at the University of Waterloo currently pursuing Mathematical Finance and Combinatorics & Optimization. I have a deep passion for mathematics and I aspire to apply my technical and mathematical skills in software development, quantitative research, and cryptography.
        </p>

        <p>
          As a kid growing up, I remember spending hours playing Pokemon on my 3DS. I think my interest in mathematics began with that. I spent time thinking through team optimization and probability calculations trying to hunt for some "shinies".
        </p>

        <p>
          My hobbies other than video games include playing basketball, swimming, reading, and hitting the gym. I love to learn and challenge myself whether through school or doing some cool projects. I'm excited for what's to come in the future and the impact I can make with mathematics.
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
