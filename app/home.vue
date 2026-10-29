```vue
<template>
  <div class="portfolio">

    <!-- Navigation -->
    <header class="navbar">
      <div class="container nav-content">
        <h1 class="logo">NICO.</h1>

        <nav>
          <a href="#home">Home</a>
          <a href="#about">About</a>
          <a href="#skills">Skills</a>
          <a href="#projects">Projects</a>
          <a href="#contact">Contact</a>
        </nav>
      </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
      <div class="container hero-content">

        <div class="hero-text">
          <p class="intro">Hello, I'm</p>

          <h2>
            Nico <span>Nuñez</span>
          </h2>

          <h3>BSIT Student & Aspiring Web Developer</h3>

          <p class="description">
            I am an Information Technology student interested in web
            development, database systems, and creating practical
            technology solutions.
          </p>

          <div class="hero-buttons">
            <a href="#projects" class="btn primary">
              View My Projects
            </a>

            <a href="#contact" class="btn secondary">
              Contact Me
            </a>
          </div>
        </div>

        <div class="hero-card">
          <div class="profile-circle">
            NN
          </div>
        </div>

      </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section">
      <div class="container">

        <p class="section-label">ABOUT ME</p>

        <h2 class="section-title">
          A student passionate about technology
        </h2>

        <div class="about-content">

          <div>
            <p>
              I am currently pursuing a Bachelor of Science in Information
              Technology. I enjoy learning how software and technology can
              be used to solve real-world problems.
            </p>

            <p>
              My interests include frontend development, backend systems,
              database management, UI/UX design, and developing
              user-friendly applications.
            </p>
          </div>

          <div class="about-info">
            <div>
              <strong>Education</strong>
              <span>BS Information Technology</span>
            </div>

            <div>
              <strong>Focus</strong>
              <span>Web Development</span>
            </div>

            <div>
              <strong>Location</strong>
              <span>Philippines</span>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="section skills-section">
      <div class="container">

        <p class="section-label">MY SKILLS</p>

        <h2 class="section-title">
          Technologies I work with
        </h2>

        <div class="skills-grid">

          <div class="skill-card">
            <div class="skill-icon">&lt;/&gt;</div>
            <h3>Frontend Development</h3>
            <p>
              HTML, CSS, JavaScript, Vue.js, and Nuxt.
            </p>
          </div>

          <div class="skill-card">
            <div class="skill-icon">DB</div>
            <h3>Database</h3>
            <p>
              PostgreSQL and relational database management.
            </p>
          </div>

          <div class="skill-card">
            <div class="skill-icon">JV</div>
            <h3>Programming</h3>
            <p>
              Java and object-oriented programming.
            </p>
          </div>

          <div class="skill-card">
            <div class="skill-icon">UI</div>
            <h3>UI/UX Design</h3>
            <p>
              Designing simple and user-friendly interfaces.
            </p>
          </div>

        </div>
      </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="section">
      <div class="container">

        <p class="section-label">MY WORK</p>

        <h2 class="section-title">
          Featured Projects
        </h2>

        <div class="projects-grid">

          <article class="project-card">
            <div class="project-number">01</div>

            <h3>Barangay Information System</h3>

            <p>
              An AI-assisted web-based information and resident services
              system designed to help improve information access and
              communication for barangay residents.
            </p>

            <div class="project-tags">
              <span>Nuxt</span>
              <span>AI</span>
              <span>Web</span>
            </div>
          </article>

          <article class="project-card">
            <div class="project-number">02</div>

            <h3>Bank Database System</h3>

            <p>
              A Java-based database application designed to manage
              customers, accounts, branches, and loans.
            </p>

            <div class="project-tags">
              <span>Java</span>
              <span>PostgreSQL</span>
              <span>NetBeans</span>
            </div>
          </article>

          <article class="project-card">
            <div class="project-number">03</div>

            <h3>Travel Application</h3>

            <p>
              A mobile application interface created to provide users with
              a simple and engaging travel experience.
            </p>

            <div class="project-tags">
              <span>Android</span>
              <span>Java</span>
              <span>UI/UX</span>
            </div>
          </article>

        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
      <div class="container contact-content">

        <p class="section-label">CONTACT</p>

        <h2>
          Let's build something together.
        </h2>

        <p>
          If you would like to connect with me or discuss a project,
          feel free to reach out.
        </p>

        <a
          href="mailto:your-email@example.com"
          class="btn primary"
        >
          Email Me
        </a>

      </div>
    </section>

    <!-- Footer -->
    <footer>
      <div class="container">
        <p>© 2026 Nico Nuñez. All rights reserved.</p>
      </div>
    </footer>

  </div>
</template>

<style scoped>
/* =========================
   General
========================= */

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  scroll-behavior: smooth;
}

.portfolio {
  min-height: 100vh;
  background: #f8fafc;
  color: #0f172a;
  font-family: Arial, Helvetica, sans-serif;
}

.container {
  width: min(1100px, 90%);
  margin: auto;
}

/* =========================
   Navigation
========================= */

.navbar {
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(255, 255, 255, 0.95);
  border-bottom: 1px solid #e2e8f0;
  backdrop-filter: blur(10px);
}

.nav-content {
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  font-size: 24px;
  letter-spacing: 2px;
}

nav {
  display: flex;
  gap: 28px;
}

nav a {
  color: #475569;
  text-decoration: none;
  font-size: 14px;
  transition: 0.2s;
}

nav a:hover {
  color: #2563eb;
}

/* =========================
   Hero
========================= */

.hero {
  min-height: 650px;
  display: flex;
  align-items: center;
  background:
    radial-gradient(
      circle at 80% 20%,
      #dbeafe,
      transparent 30%
    ),
    #f8fafc;
}

.hero-content {
  display: grid;
  grid-template-columns: 1.4fr 0.6fr;
  align-items: center;
  gap: 50px;
}

.intro {
  color: #2563eb;
  font-weight: bold;
  margin-bottom: 12px;
}

.hero h2 {
  font-size: clamp(48px, 8vw, 80px);
  line-height: 1;
  margin-bottom: 20px;
}

.hero h2 span {
  color: #2563eb;
}

.hero h3 {
  font-size: 24px;
  color: #334155;
  margin-bottom: 20px;
}

.description {
  max-width: 600px;
  line-height: 1.8;
  color: #64748b;
  font-size: 17px;
}

.hero-buttons {
  display: flex;
  gap: 15px;
  margin-top: 30px;
}

/* =========================
   Buttons
========================= */

.btn {
  display: inline-block;
  padding: 13px 22px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: bold;
  transition: 0.2s;
}

.primary {
  background: #2563eb;
  color: white;
}

.primary:hover {
  background: #1d4ed8;
  transform: translateY(-2px);
}

.secondary {
  border: 1px solid #cbd5e1;
  color: #334155;
  background: white;
}

.secondary:hover {
  border-color: #2563eb;
  color: #2563eb;
}

/* =========================
   Profile
========================= */

.hero-card {
  display: flex;
  justify-content: center;
}

.profile-circle {
  width: 260px;
  height: 260px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #2563eb;
  color: white;
  font-size: 70px;
  font-weight: bold;
  box-shadow: 0 30px 60px rgba(37, 99, 235, 0.25);
}

/* =========================
   Sections
========================= */

.section {
  padding: 100px 0;
}

.section-label {
  color: #2563eb;
  font-size: 13px;
  font-weight: bold;
  letter-spacing: 2px;
  margin-bottom: 15px;
}

.section-title {
  font-size: 40px;
  max-width: 700px;
  margin-bottom: 50px;
}

/* =========================
   About
========================= */

.about-content {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 70px;
}

.about-content p {
  color: #64748b;
  line-height: 1.8;
  margin-bottom: 20px;
}

.about-info {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.about-info div {
  padding: 20px;
  background: white;
  border: 1px solid #e2e8f0;
  border-radius: 10px;
}

.about-info strong,
.about-info span {
  display: block;
}

.about-info strong {
  margin-bottom: 5px;
}

.about-info span {
  color: #64748b;
}

/* =========================
   Skills
========================= */

.skills-section {
  background: #0f172a;
  color: white;
}

.skills-section .section-title {
  color: white;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}

.skill-card {
  padding: 28px;
  border: 1px solid #334155;
  border-radius: 12px;
  background: #1e293b;
}

.skill-icon {
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 10px;
  background: #2563eb;
  font-weight: bold;
  margin-bottom: 20px;
}

.skill-card h3 {
  margin-bottom: 10px;
}

.skill-card p {
  color: #94a3b8;
  line-height: 1.6;
}

/* =========================
   Projects
========================= */

.projects-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 25px;
}

.project-card {
  background: white;
  padding: 30px;
  border: 1px solid #e2e8f0;
  border-radius: 12px;
  transition: 0.2s;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 30px rgba(15, 23, 42, 0.08);
}

.project-number {
  color: #2563eb;
  font-weight: bold;
  margin-bottom: 30px;
}

.project-card h3 {
  font-size: 22px;
  margin-bottom: 15px;
}

.project-card p {
  color: #64748b;
  line-height: 1.7;
  margin-bottom: 25px;
}

.project-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.project-tags span {
  padding: 6px 10px;
  border-radius: 5px;
  background: #eff6ff;
  color: #2563eb;
  font-size: 12px;
}

/* =========================
   Contact
========================= */

.contact-section {
  padding: 110px 0;
  background: #dbeafe;
}

.contact-content {
  text-align: center;
  max-width: 700px;
}

.contact-content .section-label {
  margin-bottom: 20px;
}

.contact-content h2 {
  font-size: 45px;
  margin-bottom: 20px;
}

.contact-content p {
  color: #475569;
  line-height: 1.7;
  margin-bottom: 30px;
}

/* =========================
   Footer
========================= */

footer {
  padding: 25px 0;
  background: #020617;
  color: #94a3b8;
  text-align: center;
  font-size: 13px;
}

/* =========================
   Responsive
========================= */

@media (max-width: 800px) {

  .nav-content {
    height: auto;
    padding: 20px 0;
    flex-direction: column;
    gap: 15px;
  }

  nav {
    gap: 15px;
    flex-wrap: wrap;
    justify-content: center;
  }

  .hero {
    padding: 80px 0;
  }

  .hero-content {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .description {
    margin: auto;
  }

  .hero-buttons {
    justify-content: center;
    flex-wrap: wrap;
  }

  .hero-card {
    order: -1;
  }

  .profile-circle {
    width: 180px;
    height: 180px;
    font-size: 50px;
  }

  .about-content {
    grid-template-columns: 1fr;
  }

  .skills-grid {
    grid-template-columns: 1fr 1fr;
  }

  .projects-grid {
    grid-template-columns: 1fr;
  }

  .section-title {
    font-size: 32px;
  }

  .contact-content h2 {
    font-size: 35px;
  }
}

@media (max-width: 500px) {

  .skills-grid {
    grid-template-columns: 1fr;
  }

  .hero h2 {
    font-size: 50px;
  }

  .hero h3 {
    font-size: 20px;
  }
}
</style>
```