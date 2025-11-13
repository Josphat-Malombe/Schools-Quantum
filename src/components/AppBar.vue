<template>
  <header :class="['navbar', { scrolled: isScrolled }]">
    <div class="logo">
      <span class="logo-highlight">Quantum</span> Ripple
    </div>

    <nav :class="['nav-links', { open: isMenuOpen }]">
      <a href="#home" @click="closeMenu">Home</a>
      <a href="#why" @click="closeMenu">Why Us</a>
      <a href="#website" @click="closeMenu">Website</a>
      <a href="#portals" @click="closeMenu">Portals</a>
      <a href="#contact" @click="closeMenu">Contact</a>
    </nav>

    <div class="menu-icon" @click="toggleMenu">
      <div :class="{ 'bar1': true, 'change': isMenuOpen }"></div>
      <div :class="{ 'bar2': true, 'change': isMenuOpen }"></div>
      <div :class="{ 'bar3': true, 'change': isMenuOpen }"></div>
    </div>
  </header>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const isMenuOpen = ref(false)
const toggleMenu = () => (isMenuOpen.value = !isMenuOpen.value)
const closeMenu = () => (isMenuOpen.value = false)

const isScrolled = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Poppins:wght@500;600;700&display=swap');

.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 1.8rem 0;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(135deg, #0a0f24 0%, #0c1e40 100%);
  backdrop-filter: blur(12px);
  box-shadow: 0 4px 25px rgba(0, 0, 0, 0.4);
  border-bottom: 1px solid rgba(255, 255, 255, 0.08);
  z-index: 1000;
  transition: all 0.3s ease;
  font-family: 'Poppins', 'Inter', sans-serif;
}

.logo {
  position: absolute;
  left: 3rem;
  font-size: 1.9rem;
  font-weight: 700;
  color: #f5f8fa;
  letter-spacing: 0.5px;
  cursor: pointer;
  user-select: none;
  text-transform: uppercase;
}

.logo-highlight {
  color: #00d9ff;
  text-shadow: 0 0 12px rgba(0, 217, 255, 0.6);
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 2rem;
}

.nav-links a {
  position: relative;
  text-decoration: none;
  color: #e2e8f0;
  font-weight: 500;
  font-size: 1rem;
  letter-spacing: 0.3px;
  transition: color 0.3s ease, transform 0.2s ease;
}

.nav-links a::after {
  content: '';
  position: absolute;
  left: 0;
  bottom: -6px;
  width: 0%;
  height: 2px;
  background: #00d9ff;
  border-radius: 1px;
  transition: width 0.3s ease;
}

.nav-links a:hover {
  color: #00d9ff;
  transform: translateY(-2px);
}

.nav-links a:hover::after {
  width: 100%;
}

.menu-icon {
  display: none;
  flex-direction: column;
  cursor: pointer;
  gap: 6px;
  position: absolute;
  right: 3rem;
  z-index: 1100;
}

.menu-icon div {
  width: 28px;
  height: 3px;
  background: white;
  border-radius: 2px;
  transition: 0.4s;
}

.bar1.change {
  transform: rotate(-45deg) translate(-5px, 6px);
}
.bar2.change {
  opacity: 0;
}
.bar3.change {
  transform: rotate(45deg) translate(-5px, -6px);
}

@media (max-width: 900px) {
  .nav-links {
    position: absolute;
    top: 80px;
    right: 0;
    flex-direction: column;
    background: rgba(15, 20, 40, 0.98);
    width: 240px;
    padding: 2rem 1.5rem;
    gap: 1.5rem;
    border-left: 1px solid rgba(255, 255, 255, 0.08);
    opacity: 0;
    transform: translateX(100%);
    transition: all 0.4s ease;
    box-shadow: -4px 0 20px rgba(0, 0, 0, 0.3);
  }

  .nav-links.open {
    opacity: 1;
    transform: translateX(0);
  }

  .menu-icon {
    display: flex;
  }

  .nav-links a {
    font-size: 1.1rem;
  }
}

.navbar.scrolled {
  background: rgba(10, 15, 35, 0.95);
  padding: 1.2rem 3rem;
  transition: all 0.3s ease;
}
</style>