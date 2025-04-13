<template>
  <div class="project-card">
    <img :src="image" :alt="title" class="project-image" />
    <div class="project-content">
      <h2 class="project-title">{{ title }}</h2>
      <p class="project-description">{{ desc }} </p>
      <a :href="github" target="_blank" class="github-link">View on GitHub</a>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  image: String,
  github: String,
  desc: String,
})
</script>

<style scoped>
.project-card {
  background-color: #1e1e1e;
  padding: 1.5rem;
  border-radius: 1rem;
  margin-bottom: 4rem;
  box-shadow: 0 0 2rem var(--accent-color);
  display: flex;
  flex-direction: column;
  align-items: center;
  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease;
  animation: fadeInUp 0.6s ease forwards;
  gap: 1rem;
}

.project-card:hover {
  transform: translateY(-8px) scale(1.02);
  box-shadow: 0 0 4rem var(--accent-color);
  cursor: pointer;
}

.project-image {
  border-radius: 20px;
  width: 100%;
  max-width: 400px;
  height: auto;
  object-fit: cover;
  margin-top: 1rem;
  margin-bottom: 1rem;
}

.project-content {
  text-align: center;
}

.project-title {
  font-size: 1.25rem;
  font-weight: bold;
}

.project-description {
align-text: center;
  font-size: 1rem;
  margin-bottom: 1rem;
  line-height: 1.4;
}

.github-link {
  font-size: 1rem;
  transition: all 0.3s ease;
}

.github-link:hover {
  text-shadow:
    0 0 8px #42b883,
    0 0 15px #42b883;
}
</style>
