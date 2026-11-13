<script setup>
useHead({ title: 'Nico Nuñez | Home' })
</script>

<template>
  <section class="hero">
    <div class="hero-content">
      <h1>Hi, I'm Nico Nuñez</h1>
      <p>Aspiring Web Developer & IT Specialist</p>
      <div class="hero-buttons">
        <a href="/resume/nico-nunez-resume.pdf" target="_blank" class="btn">
          View Resume
        </a>
        <NuxtLink to="/contact" class="btn btn-outline">Contact Me</NuxtLink>
      </div>
    </div>

    <div class="hero-image">
      <img src="/images/nico-formal-nobg.png" alt="Nico Nuñez" />
    </div>
  </section>
</template>