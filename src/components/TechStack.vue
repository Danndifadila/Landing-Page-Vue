<template>
  <section>
    <h1>Tech Stack</h1>
    <div class="icon-list">
      <a
        v-for="icon in icons"
        :key="icon.name"
        :href="icon.link"
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
  { name: 'JavaScript', src: 'javascript-icon.svg', link: '#' },
  { name: 'Tailwind', src: 'tailwindcss-icon.svg', link: '#' },
  { name: 'React', src: 'reactjs-icon.svg', link: '#' },
  { name: 'Vue', src: 'vuejs-icon.svg', link: '#' },
]
</script>

<style scoped>
section {
  margin-top: 2rem;
  margin-bottom: 4rem;
  padding: 1rem;
  text-align: center;
}

h1 {
  font-size: 2rem;
  margin-bottom: 2rem;
}

.icon-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem;
}

.icon {
  font-size: 3rem;
  transition: all 0.3s ease;
}

.icon:hover {
  cursor: pointer;
  color: var(--accent-color);
  transform: translateY(-8px) scale(1.05);
  text-shadow:
    0 0 2rem var(--accent-color),
    0 0 15px var(--accent-color),
    0 0 25px var(--accent-color);
}

@media (min-width: 768px) {
  h1 {
    font-size: 2.5rem;
  }

  .icon {
    font-size: 4rem;
  }
}
</style>
