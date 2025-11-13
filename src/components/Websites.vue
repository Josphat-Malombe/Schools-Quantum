<template>
  <section id="website" class="website-page">
    <div class="section">
      <h2>Website Plans</h2>
      <p>Choose a plan that suits your school’s digital presence. Scalable, professional, and fully customizable.</p>

      <div class="cards">
        <div class="card basic">
          <h3>Basic Plan</h3>
          <p class="price">KES 30,000</p>
          <ul>
            <li>Homepage</li>
            <li>About Us</li>
            <li>Contact Page</li>
            <li>Photo & Video Gallery</li>
            <li>Social Media Links</li>
            <li>Responsive Design</li>
            <li>Basic SEO Setup</li>
          </ul>
          <a href="#contact" class="cta-btn">Get Started</a>
        </div>

<div class="card pro">
  <div class="ribbon">Most Popular</div>
  <h3>Pro Plan</h3>
  <p class="price">KES 45,000</p>
  <ul>
    <li>All Basic Features</li>
    <li>Digital Calendar & Events</li>
    <li>Resource Center</li>
    <li>Online Admissions</li>
    <li>News & Events</li>
    <li>Contact Forms & Google Maps</li>
    <li>Testimonials</li>
    <li>Staff/Faculty Directory</li>
    <li>Students Corner</li>
  </ul>
  <a href="#contact" class="cta-btn">Get Started</a>
</div>


        <div class="card max">
          <h3>Max Plan</h3>
          <p class="price">KES 60,000</p>
          <ul>
            <li>All Pro Features</li>
            <li>AI Agent Customer Support</li>
            <li>Blog Platform</li>
            <li>Multilingual Support</li>
            <li>Large Gallery</li>
            <li>Virtual Tours</li>
          </ul>
          <a href="#contact" class="cta-btn">Get Started</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');

.website-page {
  font-family: 'Poppins', sans-serif;
  padding: 6rem 2rem;
  background: #f5f7fa;
  color: #1e1e1e;
}

.section {
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
  padding-top: 0px;
}

.section h2 {
  font-size: 3rem;
  color: #0a5c82;
  margin-bottom: 1rem;
  font-weight: 700;
}

.section p {
  font-size: 1.15rem;
  color: #555;
  margin-bottom: 3rem;
  line-height: 1.6;
}

.cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2.5rem;
  justify-items: center;
  align-items: stretch;
}

.card {
  background: transparent;
  border-radius: 20px;
  padding: 2rem 1.5rem;
  border: 2px solid #d0d0d0;
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: all 0.3s ease;
  width: 100%;
  max-width: 350px;
}

.card:hover {
  transform: translateY(-5px);
  border-color: #0a5c82;
  box-shadow: 0 10px 25px rgba(10, 92, 130, 0.1);
}

.card h3 {
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
  color: #0a5c82;
}

.price {
  font-size: 1.45rem;
  font-weight: 700;
  margin-bottom: 1.5rem;
  color: #00d9ff;
}

.card ul {
  list-style: none;
  padding: 0;
  margin-bottom: 2rem;
  width: 100%;
}

.card ul li {
  font-size: 1rem;
  margin: 0.5rem 0;
  color: #555;
  text-align: left;
  padding-left: 1rem;
  position: relative;
}

.card ul li::before {
  content: "•";
  color: #00d9ff;
  position: absolute;
  left: 0;
}

.cta-btn {
  padding: 0.8rem 1.8rem;
  border-radius: 30px;
  background: #00d9ff;
  color: #000;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
}

.cta-btn:hover {
  background: #0a5c82;
  color: #fff;
}
.ribbon {
  position: absolute;
  top: -10px;
  right: -10px;
  background: linear-gradient(45deg, #00d9ff, #0a5c82);
  color: white;
  padding: 0.4rem 1rem;
  font-size: 0.8rem;
  font-weight: 700;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
}

.card.pro {
  border: 2px solid;
  border-image: linear-gradient(45deg, #00d9ff, #0a5c82) 1;
}

.card.pro:hover {
  box-shadow: 0 12px 30px rgba(10, 92, 130, 0.2);
  transform: translateY(-6px);
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
    padding: 1.5rem 1rem;
    max-width: 90%;
  }

  .card h3 {
    font-size: 1.3rem;
  }

  .price {
    font-size: 1.25rem;
  }

  .card ul li {
    font-size: 0.9rem;
    padding-left: 0.8rem;
  }

  .cta-btn {
    font-size: 0.9rem;
    padding: 0.6rem 1.2rem;
  }
}
</style>