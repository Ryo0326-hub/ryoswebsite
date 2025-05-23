<template>
  <section id="experience" class="py-20 bg-gray-100">
    <!-- Experience Section Title -->
    <div class="section-header mb-8">
      <img 
        src="../assets/mathematics.png" 
        alt="Matrix Icon" 
        class="icon-spin-slow"
      />
      <h2>Experiences</h2>
    </div>

    <!-- Experiences Containers -->
    <div class="experience-container">
      <!-- Experience 1 -->
      <div class="experience-card">
        <h3 class="experience-title">Quantitative Analyst Intern</h3>
        <p class="experience-date text-sm italic">June 2023 - August 2023</p>
        <p>
          Assisted in developing financial models for multi-asset portfolios using Python, ensuring a 15% improvement in risk-adjusted returns.
        </p>
      </div>

      <!-- Experience 2 -->
      <div class="experience-card">
        <h3 class="experience-title">Data Scientist</h3>
        <p class="experience-date text-sm italic">January 2022 - May 2022</p>
        <p>
          Created data pipelines to analyze time series market data and built predictive models for equity derivatives.
        </p>
      </div>

      <!-- Experience 3 -->
      <div class="experience-card">
        <h3 class="experience-title">Quantitative Researcher</h3>
        <p class="experience-date text-sm italic">September 2022 - December 2022</p>
        <p>
          Designed and backtested trading strategies, achieving an annualized return of 12% on simulated data.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Experience',
})
</script>

<style scoped>
/* Experience Section */

.experience-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); /* Responsive grid */
  gap: 2rem; /* Space between cards */
  max-width: 1000px;
  margin: 0 auto; /* Center the grid */
  padding: 1rem; /* Add padding */
}

/* Paper Effect for Individual Cards */
.experience-card {
  background: #fff; /* White background to mimic paper */
  border-radius: 12px; /* Rounded corners */
  box-shadow: 0 8px 15px rgba(0, 0, 0, 0.15),
              0 4px 6px rgba(0, 0, 0, 0.1); /* Paper-like shadow */
  padding: 1.5rem;
  position: relative;
  overflow: hidden;
  transform: rotate(-1deg); /* Slight rotation for paper effect */
  font-family: 'Patrick Hand', cursive; /* Handwritten font */
  transition: transform 0.3s, box-shadow 0.3s;
}

/* Hover Effect for Cards */
.experience-card:hover {
  transform: rotate(0deg) scale(1.02); /* Rotate back and enlarge slightly */
  box-shadow: 0 12px 25px rgba(0, 0, 0, 0.3); /* Enhance shadow on hover */
}

/* Decorations for Cards */
.experience-title {
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
  text-transform: uppercase; /* Title all caps */
}

.experience-date {
  color: #a0a0a0; /* Lighter text for dates */
  margin-bottom: 1rem;
}

/* Wrinkle Effect for Paper */
.experience-card:before {
  content: '';
  position: absolute;
  height: 100%;
  width: 100%;
  top: 0;
  left: 0;
  background: radial-gradient(
    circle,
    rgba(0, 0, 0, 0) 90%,
    rgba(0, 0, 0, 0.05) 100%
  );
  pointer-events: none; /* Ensure it's not interactive */
  z-index: -1; /* Place behind the card content */
}
</style>

