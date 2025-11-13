<template>
  <section id="statistics" class="statistics-page">
    <div class="section">
      <h2>Our Statistics</h2>
      <p>See the impact Quantum Ripple is making in schools across the region.</p>

      <div class="stats-grid">
        <div class="stat-card">
          <svg xmlns="http://www.w3.org/2000/svg" class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M3 13h2v-2H3v2zm0 4h2v-2H3v2zm0-8h2V7H3v2zm4 4h14v-2H7v2zm0 4h14v-2H7v2zm0-8h14V7H7v2z"/>
          </svg>
          <h3>16</h3>
          <p>Schools</p>
        </div>

        <div class="stat-card">
          <svg xmlns="http://www.w3.org/2000/svg" class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 12c2.21 0 4-1.79 4-4S14.21 4 12 4 8 5.79 8 8s1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/>
          </svg>
          <h3>11,000+</h3>
          <p>Students</p>
        </div>

        <div class="stat-card">
          <svg xmlns="http://www.w3.org/2000/svg" class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M16 11c1.66 0 2.99-1.34 2.99-3S17.66 5 16 5s-3 1.34-3 3 1.34 3 3 3zm-8 0c1.66 0 2.99-1.34 2.99-3S9.66 5 8 5 5 6.34 5 8s1.34 3 3 3zm0 2c-2.33 0-7 1.17-7 3.5V19h14v-2.5c0-2.33-4.67-3.5-7-3.5zm8 0c-.29 0-.62.02-.97.05 1.16.84 1.97 1.97 1.97 3.45V19h6v-2.5c0-2.33-4.67-3.5-7-3.5z"/>
          </svg>
          <h3>500+</h3>
          <p>Teachers</p>
        </div>

        <div class="stat-card">
          <svg xmlns="http://www.w3.org/2000/svg" class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm6 8v-2c0-2.21-3.58-4-8-4s-8 1.79-8 4v2h16z"/>
          </svg>
          <h3>12,000+</h3>
          <p>Parents</p>
        </div>

        <div class="stat-card">
          <svg xmlns="http://www.w3.org/2000/svg" class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M20 6H4v12h16V6zm0-2c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2h16z"/>
          </svg>
          <h3>16</h3>
          <p>Websites</p>
        </div>

        <div class="stat-card">
          <svg xmlns="http://www.w3.org/2000/svg" class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M19 3H5c-1.1 0-2 .9-2 2v14l4-4h12c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2z"/>
          </svg>
          <h3>5</h3>
          <p>Portals</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');

.statistics-page {
  font-family: 'Poppins', sans-serif;
  background: #f9f9f9;
  padding: 6rem 2rem;
  color: #1e1e1e;
}

.section {
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
}

.section h2 {
  font-size: 3rem;
  color: #0a5c82;
  margin-bottom: 1rem;
  font-weight: 700;
}

.section p {
  font-size: 1.15rem;
  color: #333;
  margin-bottom: 3rem;
  line-height: 1.6;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 2rem;
  justify-items: center;
  align-items: stretch;
}

.stat-card {
  background: #f9f9f9;
  border: 2px solid #d0d0d0;
  border-radius: 15px;
  padding: 2rem 1rem;
  text-align: center;
  transition: all 0.3s ease;
}

.stat-card:hover {
  border-color: #0a5c82;
  box-shadow: 0 10px 25px rgba(10, 92, 130, 0.15);
  transform: translateY(-5px);
}

.icon {
  width: 50px;
  height: 50px;
  color: #0a5c82;
  margin-bottom: 1rem;
}

.stat-card h3 {
  font-size: 1.8rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
  color: #00d9ff;
}

.stat-card p {
  font-size: 1rem;
  color: #555;
}

@media (max-width: 1024px) {
  .stats-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 1.8rem;
  }
}

@media (max-width: 768px) {
  .stats-grid {
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
  }

  .stat-card h3 {
    font-size: 1.4rem;
  }

  .icon {
    width: 40px;
    height: 40px;
  }
}
</style>
