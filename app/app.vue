<template>
  <div class="home-page">

    <!-- Navigation -->
    <nav class="navbar">
      <div class="nav-container">

        <div class="logo">
          NICO<span>.</span>
        </div>

        <div class="nav-links">
          <a href="#home" class="active">Home</a>
          <a href="#about">About</a>
          <a href="#projects">Projects</a>
          <a href="#contact">Contact</a>
        </div>

      </div>
    </nav>


    <!-- Home / Hero Section -->
    <main id="home" class="hero">

      <div class="hero-container">

        <!-- Left Side -->
        <div class="hero-content">

          <p class="greeting">
            Hello, I'm
          </p>

          <h1>
            Nico <span>Nuñez</span>
          </h1>

          <h2>
            Information Technology Student
          </h2>

          <p class="description">
            I am an aspiring web developer passionate about creating
            modern, user-friendly, and practical digital solutions.
            I enjoy working with web technologies, databases, and
            software development.
          </p>

          <div class="buttons">

            <a href="#projects" class="btn primary">
              View My Work
            </a>

            <a href="#contact" class="btn secondary">
              Contact Me
            </a>

          </div>

        </div>


        <!-- Right Side / Profile -->
        <div class="hero-image">

          <div class="profile-wrapper">

            <div class="profile-circle">
              <span>NN</span>
            </div>

            <div class="circle-decoration decoration-one"></div>
            <div class="circle-decoration decoration-two"></div>

          </div>

        </div>

      </div>

    </main>


    <!-- Small Introduction -->
    <section class="quick-intro">

      <div class="intro-container">

        <div class="intro-item">
          <h3>Web Development</h3>
          <p>
            Building responsive and user-friendly websites.
          </p>
        </div>

        <div class="intro-item">
          <h3>UI / UX</h3>
          <p>
            Creating simple and practical user experiences.
          </p>
        </div>

        <div class="intro-item">
          <h3>Problem Solving</h3>
          <p>
            Using technology to solve real-world problems.
          </p>
        </div>

      </div>

    </section>

  </div>
</template>


<style scoped>

/* =========================
   GENERAL
========================= */

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.home-page {
  min-height: 100vh;
  background: #f8fafc;
  color: #0f172a;
  font-family: Arial, Helvetica, sans-serif;
}


/* =========================
   NAVBAR
========================= */

.navbar {
  width: 100%;
  height: 75px;
  background: rgba(255, 255, 255, 0.95);
  border-bottom: 1px solid #e2e8f0;
  position: sticky;
  top: 0;
  z-index: 100;
}

.nav-container {
  width: 90%;
  max-width: 1200px;
  height: 100%;
  margin: auto;

  display: flex;
  align-items: center;
  justify-content: space-between;
}


/* Logo */

.logo {
  font-size: 25px;
  font-weight: 800;
  letter-spacing: 2px;
}

.logo span {
  color: #2563eb;
}


/* Navigation Links */

.nav-links {
  display: flex;
  gap: 35px;
}

.nav-links a {
  color: #475569;
  text-decoration: none;
  font-size: 15px;
  font-weight: 500;
  transition: 0.2s ease;
}

.nav-links a:hover {
  color: #2563eb;
}

.nav-links a.active {
  color: #2563eb;
  font-weight: 700;
}


/* =========================
   HERO
========================= */

.hero {
  min-height: calc(100vh - 75px);

  display: flex;
  align-items: center;

  background:
    radial-gradient(
      circle at 80% 30%,
      #dbeafe 0%,
      transparent 30%
    ),
    #f8fafc;
}


.hero-container {
  width: 90%;
  max-width: 1200px;
  margin: auto;

  display: grid;
  grid-template-columns: 1.2fr 0.8fr;

  align-items: center;

  gap: 70px;
}


/* =========================
   HERO CONTENT
========================= */

.hero-content {
  max-width: 650px;
}


.greeting {
  color: #2563eb;
  font-size: 18px;
  font-weight: 700;

  margin-bottom: 15px;
}


.hero h1 {
  font-size: clamp(55px, 7vw, 85px);
  line-height: 1;

  margin-bottom: 20px;
}


.hero h1 span {
  color: #2563eb;
}


.hero h2 {
  font-size: 25px;
  font-weight: 500;

  color: #334155;

  margin-bottom: 25px;
}


.description {
  max-width: 600px;

  color: #64748b;

  font-size: 17px;
  line-height: 1.8;
}


/* =========================
   BUTTONS
========================= */

.buttons {
  display: flex;
  gap: 15px;

  margin-top: 35px;
}


.btn {
  display: inline-block;

  padding: 14px 24px;

  border-radius: 8px;

  text-decoration: none;

  font-weight: 700;

  transition: 0.2s ease;
}


.btn.primary {
  background: #2563eb;
  color: white;
}


.btn.primary:hover {
  background: #1d4ed8;
  transform: translateY(-2px);
}


.btn.secondary {
  background: white;

  color: #334155;

  border: 1px solid #cbd5e1;
}


.btn.secondary:hover {
  border-color: #2563eb;
  color: #2563eb;
}


/* =========================
   PROFILE AREA
========================= */

.hero-image {
  display: flex;
  justify-content: center;
  align-items: center;
}


.profile-wrapper {
  width: 350px;
  height: 350px;

  position: relative;

  display: flex;
  justify-content: center;
  align-items: center;
}


/* Main Circle */

.profile-circle {
  width: 280px;
  height: 280px;

  border-radius: 50%;

  background: #2563eb;

  display: flex;
  justify-content: center;
  align-items: center;

  color: white;

  font-size: 75px;
  font-weight: 800;

  box-shadow:
    0 25px 60px rgba(37, 99, 235, 0.25);
}


.profile-circle span {
  letter-spacing: 3px;
}


/* Decorative circles */

.circle-decoration {
  position: absolute;

  border-radius: 50%;

  border: 2px solid #93c5fd;
}


.decoration-one {
  width: 320px;
  height: 320px;

  top: 15px;
  left: 15px;
}


.decoration-two {
  width: 350px;
  height: 350px;

  top: 0;
  left: 0;

  border-color: #dbeafe;
}


/* =========================
   QUICK INTRO
========================= */

.quick-intro {
  background: white;

  border-top: 1px solid #e2e8f0;

  border-bottom: 1px solid #e2e8f0;
}


.intro-container {
  width: 90%;
  max-width: 1200px;

  margin: auto;

  display: grid;

  grid-template-columns: repeat(3, 1fr);

  gap: 30px;

  padding: 45px 0;
}


.intro-item {
  padding: 10px 20px;

  border-left: 3px solid #2563eb;
}


.intro-item h3 {
  font-size: 18px;

  margin-bottom: 8px;
}


.intro-item p {
  color: #64748b;

  font-size: 14px;

  line-height: 1.6;
}


/* =========================
   RESPONSIVE
========================= */

@media (max-width: 850px) {

  .nav-links {
    gap: 15px;
  }


  .hero {
    padding: 80px 0;
  }


  .hero-container {
    grid-template-columns: 1fr;

    text-align: center;

    gap: 60px;
  }


  .hero-content {
    margin: auto;
  }


  .description {
    margin: auto;
  }


  .buttons {
    justify-content: center;
    flex-wrap: wrap;
  }


  .hero-image {
    order: -1;
  }


  .profile-wrapper {
    transform: scale(0.8);
  }


  .intro-container {
    grid-template-columns: 1fr;
  }


  .intro-item {
    text-align: left;
  }
}


@media (max-width: 500px) {

  .nav-container {
    flex-direction: column;

    justify-content: center;

    gap: 8px;
  }


  .navbar {
    height: auto;

    padding: 15px 0;
  }


  .nav-links {
    gap: 15px;
  }


  .nav-links a {
    font-size: 13px;
  }


  .hero h1 {
    font-size: 50px;
  }


  .hero h2 {
    font-size: 20px;
  }


  .profile-wrapper {
    transform: scale(0.65);
  }

}

</style>