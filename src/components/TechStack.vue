<script setup>
import { AnOutlinedJavaScript } from '@kalimahapps/vue-icons'
import { ReTailwindCssFill } from '@kalimahapps/vue-icons'
import { AkReactFill } from '@kalimahapps/vue-icons'
import { AkVueFill } from '@kalimahapps/vue-icons'
</script>

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

.icon-container {
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
