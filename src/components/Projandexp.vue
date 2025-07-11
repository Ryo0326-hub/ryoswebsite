<template>
  <section id="projandexp" class="py-10 md:py-20">
    <!-- Projects and Experiences Title with Icon -->
    <div class="section-header mb-6 md:mb-8">
      <h2>Projects and Experiences</h2>
    </div>

    <!-- Projects Section -->
    <div class="subsection-container project-banner mb-10 md:mb-16">
      <h3 class="subsection-title">Projects</h3>
      <div class="project-carousel-container">
        <div class="project-carousel" ref="carousel">
          <div class="project-card">
            <h4 class="text-lg font-semibold">Tesla Stock Prediction using GAN</h4>
            <a href="https://github.com/Ryo0326-hub/tesla-gan/tree/master" target="_blank" class="text-blue-600 underline">View on GitHub</a>
          </div>
          <div class="project-card">
            <h4 class="text-lg font-semibold">Tesla Stock Prediction using LSTM</h4>
            <a href="https://github.com/Ryo0326-hub/tesla-lstm/tree/master" target="_blank" class="text-blue-600 underline">View on GitHub</a>
          </div>
          <div class="project-card">
            <h4 class="text-lg font-semibold">UWJSA Website</h4>
            <a href="https://github.com/Ryo0326-hub/uwjsa-website" target="_blank" class="text-blue-600 underline">View on GitHub</a>
          </div>
          <div class="project-card">
            <h4 class="text-lg font-semibold">Pizza order Agent</h4>
            <a href="https://github.com/Ryo0326-hub/pizza-order-bot" target="_blank" class="text-blue-600 underline">View on GitHub</a>
          </div>
        </div>
      </div>
    </div>

    <!-- Experiences Section -->
    <div class="subsection-container pb-16 md:pb-20">
      <h3 class="subsection-title">Experiences</h3>
      <div class="experience-list">
        <!-- Experience 1 -->
        <div class="experience-item">
          <div class="experience-header">
            <h4 class="experience-role">Web Developer</h4>
            <span class="experience-period">Dec 2024 - Current</span>
          </div>
          <div class="experience-company">Japanese Student Association Club</div>
          <div class="experience-description">
            Developing and maintaining the club's website, implementing modern web technologies and responsive design.
          </div>
        </div>

        <!-- Experience 2 -->
        <div class="experience-item">
          <div class="experience-header">
            <h4 class="experience-role">Head of Finance</h4>
            <span class="experience-period">April 2024 - Current</span>
          </div>
          <div class="experience-company">Japanese Student Association Club</div>
          <div class="experience-description">
            Managing club finances, budgeting, and financial planning. Overseeing financial operations and ensuring fiscal responsibility.
          </div>
        </div>

        <!-- Experience 3 -->
        <div class="experience-item">
          <div class="experience-header">
            <h4 class="experience-role">Quantitative Analyst</h4>
            <span class="experience-period">Oct 2024 - Dec 2024</span>
          </div>
          <div class="experience-company">Stock Club</div>
          <div class="experience-description">
            Conducted quantitative analysis of financial markets, developed trading strategies, and performed risk assessment using statistical models.
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Projandexp'
})
</script>

<style scoped>
/* Mobile-first subsection styling */
.subsection-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 0.5rem; /* Smaller padding on mobile */
}

.subsection-title {
  font-size: 1.5rem; /* Smaller on mobile */
  font-weight: 700;
  text-align: center;
  margin-bottom: 1.5rem; /* Smaller margin on mobile */
  color: #374151;
  padding: 0; /* Remove padding that was causing centering issues */
  width: 100%; /* Ensure full width for proper centering */
}

/* Project carousel container */
.project-carousel-container {
  width: 100%;
  overflow: hidden;
}

/* Mobile-first projects carousel styling */
.project-carousel {
  display: flex;
  gap: 1rem; /* Smaller gap on mobile */
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  padding: 1rem 1.5rem; /* Added more side padding on mobile */
  margin: 0 auto;
  max-width: 100%; /* Full width on mobile */
  scrollbar-width: none; /* Firefox */
  -ms-overflow-style: none; /* IE and Edge */
}

.project-carousel::-webkit-scrollbar {
  display: none; /* Chrome, Safari, Opera */
}

.project-card {
  flex: 0 0 280px; /* Slightly smaller on mobile */
  scroll-snap-align: start;
  background: white;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Lighter shadow on mobile */
  padding: 1rem; /* Smaller padding on mobile */
  text-align: center;
  transition: transform 0.3s;
  height: 160px; /* Smaller height on mobile */
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.project-card:hover {
  transform: scale(1.02); /* Less dramatic scale on mobile */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
}

/* Desktop styles */
@media (min-width: 768px) {
  .subsection-container {
    padding: 0 1rem; /* Desktop padding */
  }

  .subsection-title {
    font-size: 1.875rem; /* Desktop font size */
    margin-bottom: 2rem; /* Desktop margin */
    padding: 0; /* Keep no padding on desktop */
  }

  .project-carousel {
    gap: 1.5rem; /* Desktop gap */
    padding: 1rem 2rem; /* Desktop padding */
    max-width: 90%; /* Desktop max-width */
  }

  .project-card {
    flex: 0 0 300px; /* Desktop width */
    padding: 1.5rem; /* Desktop padding */
    height: 180px; /* Desktop height */
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Desktop shadow */
  }

  .project-card:hover {
    transform: scale(1.05); /* Desktop scale */
    box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2); /* Desktop hover shadow */
  }
}

/* Resume-style experience list */
.experience-list {
  max-width: 800px;
  margin: 0 auto;
  padding: 0 1rem;
}

.experience-item {
  background: white;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 1.5rem;
  margin-bottom: 1.5rem;
  border-left: 4px solid #4682B4;
}

.experience-item:last-child {
  margin-bottom: 2rem; /* Add bottom margin to last experience item */
}

.experience-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 0.5rem;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.experience-role {
  font-size: 1.25rem;
  font-weight: 700;
  color: #374151;
  margin: 0;
  flex: 1;
  min-width: 200px;
}

.experience-period {
  font-size: 0.875rem;
  color: #6b7280;
  font-weight: 500;
  background: #f3f4f6;
  padding: 0.25rem 0.75rem;
  border-radius: 12px;
  white-space: nowrap;
}

.experience-company {
  font-size: 1rem;
  font-weight: 600;
  color: #4682B4;
  margin-bottom: 0.75rem;
}

.experience-description {
  font-size: 0.95rem;
  color: #6b7280;
  line-height: 1.6;
}

/* Mobile adjustments */
@media (max-width: 640px) {
  .experience-item {
    padding: 1rem;
    margin-bottom: 1rem;
  }

  .experience-header {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.25rem;
  }

  .experience-role {
    font-size: 1.125rem;
    min-width: auto;
  }

  .experience-period {
    font-size: 0.8rem;
    align-self: flex-start;
  }

  .experience-company {
    font-size: 0.9rem;
    margin-bottom: 0.5rem;
  }

  .experience-description {
    font-size: 0.875rem;
  }
}

.project-banner {
  background: url('../assets/grid.jpg') center center / cover no-repeat;
  border-radius: 12px;
  margin-bottom: 2rem;
  padding: 2rem;
  position: relative;
  z-index: 1;
}
</style>
