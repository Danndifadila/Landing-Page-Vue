<template>
  <section class="my-projects">
    <h1 class="section-title">Project</h1>
    <div class="project-list">
      <MyProjectSection title="Notes App" :image="notesImg" />
      <MyProjectSection title="Bookshelf" :image="bookshelfImg" />
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

.project-list {
display: flex;
flex-direction: column;
gap: 2rem;
}
</style>
