<template>
  <section id="portals" class="portals-page">

    <div class="section">
      <h2>School Management Portals</h2>
      <p>
        Choose the combination of portals that fit your school's needs. Each portal comes with core features to streamline operations.
      </p>

      <div class="cards">
        <div class="card principal">
          <h3>Principals Portal</h3>
          <p class="price">KES 15,000</p>
          <p class="description">Manage school operations, view reports, and oversee all activities efficiently.</p>
        </div>

        <div class="card teacher">
          <h3>Teachers Portal</h3>
          <p class="price">KES 10,000</p>
          <p class="description">Track attendance, submit grades, and manage class resources easily.</p>
        </div>

        <div class="card finance">
          <h3>Finance Portal</h3>
          <p class="price">KES 15,000</p>
          <p class="description">Manage fees, generate invoices, track payments, and generate financial reports.</p>
        </div>

        <div class="card parents">
          <h3>Parents Portal</h3>
          <p class="price">KES 10,000</p>
          <p class="description">Stay updated with student progress, attendance, and communicate with teachers.</p>
        </div>

        <div class="card students">
          <h3>Students Portal</h3>
          <p class="price">KES 10,000</p>
          <p class="description">Access assignments, grades, schedules, and communicate with teachers and peers.</p>
        </div>
      </div>
    </div>

  </section>
</template>

<script setup></script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');

.portals-page {
  font-family: 'Poppins', sans-serif;
  padding: 6rem 2rem;
  background: #f9f9f9;
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

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2.5rem;
  justify-items: center;
  align-items: stretch;
}

.card {
  background: transparent;
  border: 2px solid #d0d0d0;
  border-radius: 15px;
  padding: 2rem 1.5rem;
  text-align: center;
  transition: all 0.3s ease;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.card:hover {
  border-color: #0a5c82;
  box-shadow: 0 10px 25px rgba(10, 92, 130, 0.15);
  transform: translateY(-5px);
}

.card h3 {
  font-size: 1.4rem;
  font-weight: 600;
  margin-bottom: 0.8rem;
  color: #0a5c82;
}

.price {
  font-size: 1.2rem;
  font-weight: 700;
  margin-bottom: 1rem;
  color: #00d9ff;
}

.description {
  font-size: 1rem;
  color: #555;
  line-height: 1.6;
  max-width: 260px;
}

@media (max-width: 1024px) {
  .cards {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 768px) {
  .cards {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }

  .card {
    padding: 1.8rem 1rem;
  }

  .card h3 {
    font-size: 1.3rem;
  }

  .price {
    font-size: 1.1rem;
  }

  .description {
    font-size: 0.95rem;
  }
}
</style>