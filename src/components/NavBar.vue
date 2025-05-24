<template>
  <nav>
    <ul class="nav-list">
      <li><a href="#hero"       class="nav-link">Home</a></li>
      <li><a href="#about"      class="nav-link">About</a></li>
      <li><a href="#projandexp" class="nav-link">Projects and Experiences</a></li>
    </ul>
  </nav>
</template>

<script setup lang="ts">
  // no script needed here
</script>

<style scoped>
/* remove bullets, center items in one row, fixed gap */
.nav-list {
  list-style: none;
  margin: 0;
  padding: 1rem 0;
  display: flex;
  justify-content: center;
  gap: 2rem;             /* fixed spacing */
}

/* dark-blue text, a bit larger, hover to dark-gray */
.nav-link {
  color: #4682B4;        /* dark blue */
  font-size: 1.125rem;   /* ~18px = slightly larger */
  text-decoration: none;
  transition: color 0.2s;
}
.nav-link:hover {
  color: #4b5563;        /* dark gray */
}

/* make the nav background match the page background */
nav {
  position: fixed;
  top:      0;
  left:     0;         /* ← ensure this is here */
  width:    100%;      /* or 100vw if you want no horizontal scroll */
  z-index:  50;
  background-color: #F5F5F5;
}
</style>
