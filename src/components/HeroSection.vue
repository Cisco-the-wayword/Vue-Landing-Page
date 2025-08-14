<template>
  <!-- Hero Section -->
  <section class="hero-gradient min-h-screen flex items-center relative overflow-hidden pb-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
      <div class="space-y-8">
        <h1 class="text-5xl lg:text-6xl font-bold text-blue-900 leading-tight">
          Smarter Fuel Management 
          <span class="block">Starts Here</span>
        </h1>
        <h2 class="text-2xl text-blue-800 font-semibold">
          Take Control. Cut Costs. Stop Leakages.
        </h2>
        <p class="text-lg text-blue-800 max-w-xl">
          Remis is the fuel management solution trusted by leading businesses in Nigeria to eliminate fuel-related losses, improve visibility, and streamline operations — all in real time.
        </p>
        <p class="text-blue-800">
          Perfect for fleet managers, logistics managers, operations heads, and finance teams.
        </p>
        
        <!-- App Store Badges -->
        <div class="flex flex-col sm:flex-row gap-4">
          <div class="flex items-center space-x-4">
            <a href="https://link-to-your-app-store">
              <img src="/public/images/app-links/app-store.png" alt="Download on the App Store badge with Apple logo" class="h-12">
            </a>
            <a href="https://link-to-your-play-store">
              <img src="/public/images/app-links/play-store.png" alt="Get it on Google Play badge with Android robot icon" class="h-12">
            </a>
          </div>
        </div>
        
        <!-- Ratings -->
        <div class="flex flex-col sm:flex-row gap-8">
          <div>
            <div class="text-3xl font-bold text-blue-900">4.5/5</div>
            <div class="flex text-orange-400 text-sm">
              ★★★★★
            </div>
            <div class="text-sm text-blue-800">On the iOS App Store</div>
          </div>
          <div>
            <div class="text-3xl font-bold text-blue-900">4.5/5</div>
            <div class="flex text-orange-400 text-sm">
              ★★★★★
            </div>
            <div class="text-sm text-blue-800">On the Google Play Store</div>
          </div>
        </div>
      </div>
      
      <div class="relative">
        <div class="floating-animation">
          <img src="/public/images/hand-holding-card.png" alt="Hand holding a blue Remis fuel card against an orange gradient background, showing modern fuel management technology" class="w-full max-w-lg mx-auto">
        </div>
      </div>
    </div>
  </section>

  <!-- Partner Stations - Positioned over hero section -->
  <section class="relative -mt-32 z-10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="bg-white rounded-2xl shadow-lg p-8">
        <h3 class="text-2xl font-bold text-blue-900 text-center mb-12">Some of our Partners Stations</h3>
        <div class="grid grid-cols-2 md:grid-cols-5 gap-8 items-center justify-items-center">
          <img src="/public/images/logos/NNPC_Logo_1.png" alt="NNPC logo - green triangular design representing Nigerian National Petroleum Corporation" class="partner-logo h-12">
          <img src="/public/images/logos/Heyden_Logo_1.png" alt="Heyden logo - red and orange text logo for fuel station partner" class="partner-logo h-12">
          <img src="/public/images/logos/BOVAS_Logo_1.png" alt="Bovas logo - circular black logo with 'B' emblem for fuel station network" class="partner-logo h-12">
          <img src="/public/images/logos/Rainoil_Logo_Coloured_1.png" alt="Rainoil logo - modern orange and black design for petroleum company" class="partner-logo h-12">
          <img src="/public/images/logos/ng-eterna-logo_1.png" alt="Eterna logo - green geometric logo design for fuel station brand" class="partner-logo h-12">
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// Hero section logic
</script>

<style scoped>
/* Component-specific styles if needed */
</style>