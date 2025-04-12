<script setup>
import {AnOutlinedJavaScript} from '@kalimahapps/vue-icons'
import  { ReTailwindCssFill } from '@kalimahapps/vue-icons'
import { AkReactFill } from '@kalimahapps/vue-icons'
import { AkVueFill } from '@kalimahapps/vue-icons'
</script>

<template>
<section>
<h1> Tech Stack </h1>
<div class="icon-container">
<AnOutlinedJavaScript class="icon"/>
<ReTailwindCssFill class="icon" />
<AkReactFill class="icon" />
<AkVueFill class="icon" />
</div>
</section>
</template>

<style scoped>
section {
justify-items: center;
height: 400px
}

.icon {
display: flex;
font-size: 4rem;
cursor: pointer;
margin-right: 5rem;
justify-content: center;
align-content: center;
}
</style>
