<template>
    <div class="project-card">
      <img :src="image" alt="My Project Image" class="project-image"  />
      <h2 class="project-title">{{ title }}</h2>
    </div>
</template>

<script setup>
defineProps({
  title: String,
  image: String
})
</script>

<style scoped>
.project-card {
margin-bottom: 4rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  border: 2px solid green;
  padding: 1.5rem;
  border-radius: 12px;
  gap: 1rem;
}

.project-image {
  width: 100%;
  max-width: 400px;
  object-fit: cover;
}

.project-title {
  font-size: 1.25rem;
  font-weight: bold;
  text-align: center;
}
</style>
