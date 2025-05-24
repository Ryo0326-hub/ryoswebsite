<template>
  <section id="projandexp" class="py-20 bg-gray-100">
    <!-- Projects and Experiences Title with Icon -->
    <div class="section-header mb-8">
      <img 
        src="../assets/pi.png" 
        alt="Pi Symbol" 
        class="icon-bounce" 
      />
      <h2>Projects and Experiences</h2>
    </div>

    <!-- Projects Section -->
    <div class="subsection-container mb-16">
      <h3 class="subsection-title">Projects</h3>
      <div class="project-carousel">
        <div class="project-card">
          <h4 class="text-lg font-semibold">Financial Risk Model</h4>
          <p class="text-sm mt-2">
            A quantitative model to forecast market risks using Python and Monte Carlo simulations.
          </p>
        </div>
        <div class="project-card">
          <h4 class="text-lg font-semibold">Portfolio Optimization</h4>
          <p class="text-sm mt-2">
            Tool for maximizing returns while managing risk using Mean-Variance Optimization.
          </p>
        </div>
        <div class="project-card">
          <h4 class="text-lg font-semibold">Trading Bot</h4>
          <p class="text-sm mt-2">
            Built a bot to execute trades automatically, integrating trading APIs and machine learning.
          </p>
        </div>
        <div class="project-card">
          <h4 class="text-lg font-semibold">Time Series Forecasting</h4>
          <p class="text-sm mt-2">
            Developed a financial time series model using ARIMA to predict stock prices.
          </p>
        </div>
      </div>
    </div>

    <!-- Experiences Section -->
    <div class="subsection-container">
      <h3 class="subsection-title">Experiences</h3>
      <div class="experience-container">
        <!-- Experience 1 -->
        <div class="experience-card">
          <h4 class="experience-title">Experience Title</h4>
          <p>
            Description will go here.
          </p>
        </div>

        <!-- Experience 2 -->
        <div class="experience-card">
          <h4 class="experience-title">Experience Title</h4>
          <p>
            Description will go here.
          </p>
        </div>

        <!-- Experience 3 -->
        <div class="experience-card">
          <h4 class="experience-title">Experience Title</h4>
          <p>
            Description will go here.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Projandexp',
})
</script>

<style scoped>
/* Subsection styling */
.subsection-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}

.subsection-title {
  font-size: 1.875rem;
  font-weight: 700;
  text-align: center;
  margin-bottom: 2rem;
  color: #374151;
}

/* Projects carousel styling */
.project-carousel {
  display: flex;
  gap: 1.5rem;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  padding: 1rem 2rem;
  margin: 0 auto;
  max-width: 90%;
}

.project-card {
  flex: 0 0 300px;
  scroll-snap-align: start;
  background: white;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 1.5rem;
  text-align: center;
  transition: transform 0.3s;
  height: 180px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.project-card:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
}

/* Experience section styling */
.experience-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  max-width: 1000px;
  margin: 0 auto;
  padding: 1rem;
}

/* Paper Effect for Individual Cards */
.experience-card {
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 8px 15px rgba(0, 0, 0, 0.15),
              0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 1.5rem;
  position: relative;
  overflow: hidden;
  transform: rotate(-1deg);
  font-family: 'Patrick Hand', cursive;
  transition: transform 0.3s, box-shadow 0.3s;
}

/* Hover Effect for Cards */
.experience-card:hover {
  transform: rotate(0deg) scale(1.02);
  box-shadow: 0 12px 25px rgba(0, 0, 0, 0.3);
}

/* Decorations for Cards */
.experience-title {
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
  text-transform: uppercase;
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
  pointer-events: none;
  z-index: -1;
}
</style>
