<script setup>
import MyPhoto from '@/assets/foto_dieng.jpg'
</script>

<template>
  <section class="HeroSec">
    <img :src="MyPhoto" alt="My Photo" />
    <section class="HeroSecText">
      <h1>Hello <strong>I'm Danndifadila</strong></h1>
      <h1>A<strong> Junior Developers</strong></h1>
      <p>I'm a Curious Programmers</p>
    </section>
  </section>
</template>

<style scoped>
.HeroSec {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 500px;
  margin-bottom: 3rem;
}

h1 {
  margin: auto;
}

img {
  width: 300px;
  height: 200px;
  object-fit: cover;
  border-radius: 10px;
  margin-right: 3rem;
}
</style>
