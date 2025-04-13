<template>
  <section>
    <h1>Tech Stack</h1>
    <div class="icon-container">
      <AnOutlinedJavaScript class="icon" />
      <ReTailwindCssFill class="icon" />
      <AkReactFill class="icon" />
      <AkVueFill class="icon" />
    </div>
  </section>
</template>

<script setup>
import { AnOutlinedJavaScript } from '@kalimahapps/vue-icons'
import { ReTailwindCssFill } from '@kalimahapps/vue-icons'
import { AkReactFill } from '@kalimahapps/vue-icons'
import { AkVueFill } from '@kalimahapps/vue-icons'
</script>

<style scoped>
section {
  margin-top: 2rem;
  margin-bottom: 4rem;
  height: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  gap: 2rem;
}

.icon-container {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 3rem;
}

.icon {
  font-size: 4rem;
  transition: all 0.3s ease;
}

.icon:hover {
  cursor: pointer;
  color: var(--accent-color);
  transform: translateY(-8px) scale(1.02);
  text-shadow:
    0 0 2rem var(--accent-color),
    0 0 15px var(--accent-color),
    0 0 25px var(--accent-color);
}
</style>
