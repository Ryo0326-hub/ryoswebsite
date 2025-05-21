<template>
  <div>
    <NavBar />
    <main class="pt-20">
      <Hero />
      <About />
      <Projects />
      <Experience />
      <Contact />
    </main>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import NavBar    from './components/NavBar.vue'
import Hero      from './components/Hero.vue'
import About     from './components/About.vue'
import Projects  from './components/Projects.vue'
import Experience from './components/Experience.vue'
import Contact   from './components/Contact.vue'

export default defineComponent({
  components: { NavBar, Hero, About, Projects, Experience, Contact }
})
</script>

