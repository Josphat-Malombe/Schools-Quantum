<template>
  <section id="why" class="why-page">

    <div class="section why-digitize">
      <h2>Why Schools Are Going Digital</h2>
      <p>
        Modern schools thrive when management is streamlined. Digitizing your school:
      </p>
      <div class="cards">
        <div class="card">
          <div class="icon">📊</div>
          <h3>Efficient Administration</h3>
          <p>Automate routine tasks like attendance, grading, and reporting.</p>
        </div>
        <div class="card">
          <div class="icon">💡</div>
          <h3>Data-Driven Decisions</h3>
          <p>Access real-time analytics to make informed choices for your school.</p>
        </div>
        <div class="card">
          <div class="icon">⏱️</div>
          <h3>Save Time & Resources</h3>
          <p>Reduce paperwork and repetitive manual processes, boosting efficiency.</p>
        </div>
        <div class="card">
          <div class="icon">🌐</div>
          <h3>Remote Accessibility</h3>
          <p>Manage your school anytime, anywhere, through the cloud.</p>
        </div>
      </div>
    </div>

    <div class="section why-quantum">
      <h2>Why Choose Quantum Ripple?</h2>
      <p>
        We offer a modern, dynamic school management system designed to be an asset to your institution.
      </p>
      <div class="cards">
        <div class="card">
          <div class="icon">⚙️</div>
          <h3>Dynamic System Approach</h3>
          <p>Our system adapts to your school's needs, providing a tailored experience for every user.</p>
        </div>
        <div class="card">
          <div class="icon">🎨</div>
          <h3>Customizable Interface</h3>
          <p>Complete flexibility to design your dashboard and user interface your way.</p>
        </div>
        <div class="card">
          <div class="icon">🕒</div>
          <h3>24/7 Tech Support</h3>
          <p>We provide round-the-clock technical assistance whenever you need it.</p>
        </div>
        <div class="card">
          <div class="icon">💾</div>
          <h3>Ownership & Security</h3>
          <p>You own the source code and cloud credentials; the system is fully yours.</p>
        </div>
        <div class="card">
          <div class="icon">💰</div>
          <h3>Cost Effective</h3>
          <p>High-end features at a fraction of the cost compared to conventional solutions.</p>
        </div>
        <div class="card">
          <div class="icon">🛠️</div>
          <h3>Maintenance & Updates</h3>
          <p>Comprehensive maintenance packages to keep your system running smoothly.</p>
        </div>
      </div>
    </div>

  </section>
</template>

<script setup></script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Poppins:wght@600;700&display=swap');

.why-page {
  font-family: 'Poppins', sans-serif;
  color: #1e1e1e;
  padding: 6rem 2rem;
  background: #f9f9f9;
}

.section {
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
}

.section h2 {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1rem;
  color: #0a5c82;
  letter-spacing: 0.5px;
}

.section p {
  font-size: 1.15rem;
  color: #333;
  margin-bottom: 3rem;
  line-height: 1.7;
}

.cards {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 2.5rem;
  justify-items: center;
  align-items: stretch;
}

.card {
  background: transparent;
  padding: 2.2rem 1.5rem;
  border-radius: 15px;
  border: 2px solid #d0d0d0;
  box-shadow: none;
  transition: all 0.3s ease;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.card:hover {
  border-color: #0a5c82;
  box-shadow: 0 10px 25px rgba(10, 92, 130, 0.15);
  transform: translateY(-5px);
}

.icon {
  font-size: 2.8rem;
  margin-bottom: 1rem;
  color: #0a5c82;
  background: transparent;
  width: 60px;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  border: 2px solid #d0d0d0;
  transition: all 0.3s ease;
}

.card:hover .icon {
  border-color: #0a5c82;
  color: #0a5c82;
}

.card h3 {
  font-size: 1.3rem;
  font-weight: 600;
  margin-bottom: 0.8rem;
  color: #0a5c82;
}

.card p {
  font-size: 1rem;
  color: #555;
  line-height: 1.6;
  max-width: 250px;
}

@media (max-width: 1024px) {
  .cards {
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
  }
}

@media (max-width: 768px) {
  .cards {
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
  }

  .card {
    padding: 1.8rem 1rem;
  }

  .icon {
    width: 50px;
    height: 50px;
    font-size: 2rem;
  }

  .card h3 {
    font-size: 1.2rem;
  }

  .card p {
    font-size: 0.95rem;
  }
}
</style>