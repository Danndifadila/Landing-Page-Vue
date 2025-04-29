<template>
  <section>
    <h1>Let's Connect!</h1>
    <div class="icons-container">
      <a
        v-for="icon in icons"
        :key="icon.name"
        :href="icon.link"
        target="_blank"
        rel="noopener noreferrer"
        class="icon-item"
      >
        <img :src="icon.src" :alt="icon.name" width="70" height="70" class="icon" />
      </a>
    </div>
  </section>
</template>

<script setup>
const icons = [
  { name: 'GitHub', src: 'github-mark-white.svg', link: 'https://github.com/Danndifadila' },
  {
    name: 'LinkedIn',
    src: 'linkedin-tile.svg',
    link: 'https://www.linkedin.com/in/danndifadila-arrasikhuuna-herwanto-44b342347/',
  },
]
</script>

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
