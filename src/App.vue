<template>
  <div id="app">
    <Navbar />
    <HeroSection />
    <FeaturesSection />
    <Footer />
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
import FeaturesSection from './components/FeaturesSection.vue'
import Footer from './components/Footer.vue'
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');

* {
  font-family: 'Inter', sans-serif;
}

.hero-gradient {
  background: linear-gradient(135deg, #FFA726 0%, #FFB74D 100%);
}

.orange-gradient {
  background: linear-gradient(135deg, #FF8A65 0%, #FFB74D 100%);
}

.blue-gradient {
  background: linear-gradient(135deg, #42A5F5 0%, #1E88E5 100%);
}

.feature-card {
  background: rgba(255, 255, 255, 0.1);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
}

.testimonial-card {
  background: #ffffff;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
  border-radius: 16px;
}

.partner-logo {
  filter: grayscale(1);
  opacity: 0.7;
  transition: all 0.3s ease;
}

.partner-logo:hover {
  filter: grayscale(0);
  opacity: 1;
}

.floating-animation {
  animation: float 6s ease-in-out infinite;
}

@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-20px); }
}

.fade-in {
  opacity: 0;
  transform: translateY(30px);
  transition: all 0.6s ease;
}

.fade-in.visible {
  opacity: 1;
  transform: translateY(0);
}
</style>

#