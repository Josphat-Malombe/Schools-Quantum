<template>
  <section id="home" class="hero-section">
    <video autoplay muted loop playsinline class="background-video">
      <source src="/10.mp4" type="video/mp4" />
      Your browser does not support the video tag.
    </video>

    <div class="overlay"></div>

    <div class="hero-content">
      <h1>Transforming School Management</h1>
      <p>Next-generation digital experience for schools and institutions.</p>
      <a href="#website" class="cta-btn">Explore More</a>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Poppins:wght@600;700&display=swap');

.hero-section {
  position: relative;
  width: 100%;
  height: 100vh;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #ffffff;
  font-family: 'Poppins', sans-serif;
}

.background-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -2;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    to bottom,
    rgba(5, 10, 25, 0.6) 20%,
    rgba(10, 15, 35, 0.8) 100%
  );
  z-index: -1;
}

.hero-content {
  max-width: 800px;
  padding: 0 1.5rem;
  animation: fadeInUp 1.2s ease forwards;
}

.hero-content h1 {
  font-size: 3.2rem;
  font-weight: 700;
  margin-bottom: 1rem;
  letter-spacing: 0.5px;
  line-height: 1.2;
  color: #f5f8fa;
}

.hero-content p {
  font-size: 1.2rem;
  font-weight: 400;
  color: #d1e0f0;
  margin-bottom: 2rem;
}

.cta-btn {
  background: linear-gradient(135deg, #00d9ff, #0077b6);
  padding: 0.9rem 1.8rem;
  border-radius: 30px;
  color: #ffffff;
  text-decoration: none;
  font-weight: 600;
  letter-spacing: 0.5px;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(0, 217, 255, 0.3);
}

.cta-btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 20px rgba(0, 217, 255, 0.5);
  background: linear-gradient(135deg, #009ec9, #005f8b);
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(25px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media (max-width: 768px) {
  .hero-content h1 {
    font-size: 2.2rem;
  }

  .hero-content p {
    font-size: 1rem;
  }
}
</style>