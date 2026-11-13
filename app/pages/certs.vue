<script setup>
useHead({ title: 'Nico Nuñez | Certifications' })

const certifications = [
  {
    title: 'Python Certification',
    image: '/images/python-cert.jpg',
    badge: '/images/pythoncert.png'
  },
  {
    title: 'Microsoft Office Specialist: PowerPoint',
    image: '/images/powerpoint-cert.jpg',
    badge: '/images/powerpointbadge.png'
  },
  {
    title: 'Microsoft Office Specialist: Word',
    image: '/images/word-cert_page.jpg',
    badge: '/images/microsoftbadge.png'
  },
  {
    title: 'Networking Certification',
    image: '/images/networkingcert.png',
    badge: null
  }
]
</script>

<template>
  <section class="certs-section">
    <h2>Certifications</h2>
    <div class="certs-grid">
      <div v-for="cert in certifications" :key="cert.title" class="cert-card">
        <img :src="cert.image" :alt="cert.title" class="cert-preview" />
        <h3>{{ cert.title }}</h3>
        <a :href="cert.image" target="_blank" class="cert-link">View Certificate</a>
      </div>
    </div>
  </section>
</template>