<script setup>
import { AkGithubFill } from '@kalimahapps/vue-icons'
import { AkLinkedinBoxFill } from '@kalimahapps/vue-icons'
</script>

<template>
  <section>
    <h1>Let's Connect!</h1>
    <div class="icons-container">
      <AkGithubFill class="icon" />
      <AkLinkedinBoxFill class="icon" />
    </div>
  </section>
</template>

<style scoped>
section {
  margin-top: 2rem;
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
  cursor: pointer;
}
</style>
