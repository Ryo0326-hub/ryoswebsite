<template>
  <section id="projects" class="py-20 bg-gray-100">
    <!-- Projects Title with Icon -->
    <div class="section-header mb-6">
      <img 
        src="../assets/pi.png" 
        alt="Pi Symbol" 
        class="icon-bounce" 
      />
      <h2>Projects</h2>
    </div>

    <!-- Projects Carousel -->
    <div class="project-carousel">
      <div class="project-card">
        <img src="https://via.placeholder.com/300x200" alt="Project 1" />
        <h3 class="text-lg font-semibold mt-4">Financial Risk Model</h3>
        <p class="text-sm mt-2">
          A quantitative model to forecast market risks using Python and Monte Carlo simulations.
        </p>
      </div>
      <div class="project-card">
        <img src="https://via.placeholder.com/300x200" alt="Project 2" />
        <h3 class="text-lg font-semibold mt-4">Portfolio Optimization</h3>
        <p class="text-sm mt-2">
          Tool for maximizing returns while managing risk using Mean-Variance Optimization.
        </p>
      </div>
      <div class="project-card">
        <img src="https://via.placeholder.com/300x200" alt="Project 3" />
        <h3 class="text-lg font-semibold mt-4">Trading Bot</h3>
        <p class="text-sm mt-2">
          Built a bot to execute trades automatically, integrating trading APIs and machine learning.
        </p>
      </div>
      <div class="project-card">
        <img src="https://via.placeholder.com/300x200" alt="Project 4" />
        <h3 class="text-lg font-semibold mt-4">Time Series Forecasting</h3>
        <p class="text-sm mt-2">
          Developed a financial time series model using ARIMA to predict stock prices.
        </p>
      </div>
      <div class="project-card">
        <img src="https://via.placeholder.com/300x200" alt="Project 5" />
        <h3 class="text-lg font-semibold mt-4">Derivative Pricing</h3>
        <p class="text-sm mt-2">
          Calculated prices of options using the Black-Scholes model and Python libraries.
        </p>
      </div>
      <div class="project-card">
        <img src="https://via.placeholder.com/300x200" alt="Project 6" />
        <h3 class="text-lg font-semibold mt-4">Backtesting Framework</h3>
        <p class="text-sm mt-2">
          A framework to test trading strategies on historical data, using Pandas and NumPy.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Projects',
})
</script>

<style scoped>
/* Section-specific scrolling styles */
.project-carousel {
  display: flex;
  gap: 1rem; /* Reduced spacing between cards */
  overflow-x: auto; /* Enable horizontal scrolling */
  scroll-snap-type: x mandatory; /* Ensure cards snap into view */
  padding: 1rem 8rem; /* Larger left & right padding for compact alignment */
}

.project-card {
  flex: 0 0 calc(25% - 1rem); /* Narrower card width */
  scroll-snap-align: start; /* Snap card to start */
  background: white;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Subtle shadow */
  padding: 1rem;
  text-align: center;
  transition: transform 0.2s;
  height: 260px; /* Smaller height */
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.project-card:hover {
  transform: scale(1.05); /* Small zoom effect */
}

.project-card img {
  width: 100%; /* Full card width */
  height: 120px; /* Smaller height for images */
  object-fit: cover; /* Ensures proportional image cropping */
  border-radius: 8px; /* Match card border radius */
}
</style>
