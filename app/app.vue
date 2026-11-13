<script setup>
import { ref } from 'vue'

// Replaces DOM manipulation from script.js for mobile menu toggling
const menuOpen = ref(false)
const toggleMenu = () => {
  menuOpen.value = !menuOpen.value
}
const closeMenu = () => {
  menuOpen.value = false
}
</script>

<template>
  <div>
    <nav class="navbar">
      <div class="logo">NICO NUÑEZ</div>

      <ul class="nav-links" id="navLinks" :class="{ active: menuOpen }">
        <li><NuxtLink to="/" @click="closeMenu">Home</NuxtLink></li>
        <li><NuxtLink to="/about" @click="closeMenu">About</NuxtLink></li>
        <li><NuxtLink to="/techstack" @click="closeMenu">Tech Stack</NuxtLink></li>
        <li><NuxtLink to="/certs" @click="closeMenu">Certifications</NuxtLink></li>
        <li><NuxtLink to="/contact" @click="closeMenu">Contact</NuxtLink></li>
      </ul>
    </nav>

    <main>
      <NuxtPage />
    </main>
  </div>
</template>