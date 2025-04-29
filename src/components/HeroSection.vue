<script setup>
import MyPhoto from '@/assets/foto_dieng.jpg'
</script>

<template>
  <section class="HeroSec">
    <img :src="MyPhoto" alt="My Photo" class="hero-img" />
    <section class="HeroSecText">
      <h1>Hello <strong>I'm Danndifadila</strong></h1>
      <h1>A<strong> Junior Developer</strong></h1>
      <p>I'm a Curious Programmer</p>
    </section>
  </section>
</template>

<style scoped>
.HeroSec {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2rem 1rem;
  flex-wrap: wrap;
  gap: 2rem;
  text-align: center;
  height: 600px;
}

.hero-img {
  width: 100%;
  max-width: 300px;
  height: 200px;
  object-fit: cover;
  border-radius: 20px;
}

.HeroSecText h1 {
  font-size: 2rem;
  margin: 0.5rem 0;
}

.HeroSecText p {
  font-size: 1.1rem;
  margin-top: 1rem;
  color: #555;
}

@media (min-width: 768px) {
  .HeroSec {
    flex-wrap: nowrap;
    text-align: left;
  }

  .HeroSecText h1 {
    font-size: 2.5rem;
  }

  .HeroSecText p {
    font-size: 1.25rem;
  }
}
</style>
