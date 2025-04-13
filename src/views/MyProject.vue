<template>
  <section class="my-projects">
    <h1 class="section-title">Project</h1>
    <div class="project-grid">
      <MyProjectSection
        title="Notes App"
        :image="notesImg"
        github="https://github.com/Danndifadila/Notes-App"
        desc="This is my submission project for Dicoding Course"
      />
      <MyProjectSection
        title="Bookshelf"
        :image="bookshelfImg"
        github="https://github.com/Danndifadila/BookShelf-Dicoding"
        desc="Where I put my notes e.g activities or plan."
      />
    </div>
  </section>
</template>

<script setup>
import MyProjectSection from '@/components/MyProjectSection.vue'
import notesImg from '@/assets/notes-app.png'
import bookshelfImg from '@/assets/bookshelf.png'
</script>

<style scoped>
.my-projects {
  padding: 2rem 1rem;
  max-width: 800px;
  margin: auto;
}

.section-title {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 2rem;
}

.project-grid {
  display: grid;
  grid-template-coloumns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}
</style>
