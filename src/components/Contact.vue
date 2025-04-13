<script setup>
import { AkGithubFill } from '@kalimahapps/vue-icons'
import { AkLinkedinBoxFill } from '@kalimahapps/vue-icons'
</script>

<template>
  <section>
    <h1>Let's Connect!</h1>
    <div class="icons-container">
      <a href="https://github.com/Danndifadila" target="_blank" class="icon-wrapper">
        <AkGithubFill class="icon" />
      </a>
      <a
        href="https://www.linkedin.com/in/danndifadila-arrasikhuuna-herwanto-44b342347/"
        target="_blank"
        class="icon-wrapper"
      >
        <AkLinkedinBoxFill class="icon" />
      </a>
    </div>
  </section>
</template>

<style scoped>
section {
  margin-top: 1rem;
  margin-bottom: 5rem;
  height: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  gap: 2rem;
}

.icons-container {
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
    0 0 8px var(--accent-color),
    0 0 15px var(--accent-color),
    0 0 25px var(--accent-color);
}
</style>
