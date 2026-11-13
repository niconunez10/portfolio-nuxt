<script setup>
useHead({ title: 'Nico Nuñez | Tech Stack' })

const stack = [
  { name: 'HTML5', iconClass: 'fab fa-html5' },
  { name: 'CSS3', iconClass: 'fab fa-css3-alt' },
  { name: 'JavaScript', iconClass: 'fab fa-js' },
  { name: 'Nuxt / Vue', iconClass: 'fab fa-vuejs' },
  { name: 'Python', iconClass: 'fab fa-python' },
  { name: 'MySQL', img: '/images/mysql-icon.png' },
  { name: 'VS Code', img: '/images/vscode-logo.png' }
]
</script>

<template>
  <section class="techstack-section">
    <h2>Tech Stack</h2>
    <div class="stack-grid">
      <div v-for="item in stack" :key="item.name" class="stack-card">
        <img v-if="item.img" :src="item.img" :alt="item.name" />
        <i v-else :class="item.iconClass"></i>
        <h3>{{ item.name }}</h3>
      </div>
    </div>
  </section>
</template>