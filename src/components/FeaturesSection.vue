<template>
  <!-- Get Started Today Section -->
  <section class="orange-gradient pt-32 pb-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
      <h2 class="text-4xl lg:text-5xl font-bold text-blue-900 mb-6">Get Started Today</h2>
      <p class="text-xl text-blue-800 mb-4">No More Guesswork. Just Complete Control.</p>
      <p class="text-lg text-blue-800 mb-16 max-w-4xl mx-auto">
        Manual fuel logs, paper vouchers, and unverifiable reports cost your business time and money.
      </p>
      <p class="text-lg text-blue-800 mb-16 max-w-4xl mx-auto">
        Remis automates your entire fueling process with secure, fuel card and voucher system that puts you in full control.
      </p>
    </div>
  </section>

  <!-- Why Remis Section -->
  <section class="orange-gradient pb-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-4xl font-bold text-blue-900 text-center mb-16">Why Remis?</h2>
      <div class="grid grid-cols-1 md:grid-cols-5 gap-8">
        <div class="text-center space-y-4 fade-in" v-for="feature in features" :key="feature.id">
          <div class="text-center space-y-4">
            <div class="w-20 h-20 mx-auto mb-6 rounded-2xl flex items-center justify-center bg-white bg-opacity-30 backdrop-blur-md">
              <img :src="feature.icon" :alt="feature.iconAlt" class="w-10 h-10">
            </div>
            <h3 class="text-lg font-bold text-blue-900 mb-3">{{ feature.title }}</h3>
            <p class="text-sm text-blue-800 leading-relaxed">{{ feature.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Who It's For Section -->
  <section class="bg-gray-50 py-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
      <h2 class="text-4xl font-bold text-blue-900 mb-8">Who It's For</h2>
      <p class="text-xl text-gray-700 mb-4 max-w-3xl mx-auto">
        Remis is built for organizations that manage vehicle fleets whether you run 10 cars or 500 trucks.
      </p>
      <p class="text-lg text-gray-600 mb-12">Ideal for:</p>
      <div class="text-lg font-semibold text-blue-900 max-w-5xl mx-auto">
        Fleet Managers • Operations/Logistics Managers • Procurement & Finance Heads • CEOs/COOs seeking transparency and cost control
      </div>
    </div>
  </section>

  <!-- Customer Logos -->
  <section class="bg-gray-50 pb-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl font-bold text-blue-900 text-center mb-16">Some of Our Esteemed Customers</h2>
      <div class="grid grid-cols-2 md:grid-cols-5 gap-12 items-center justify-items-center mb-12">
        <img v-for="logo in customerLogos.slice(0, 5)" :key="logo.id" :src="logo.src" :alt="logo.alt" class="partner-logo h-10">
      </div>
      <div class="grid grid-cols-2 md:grid-cols-5 gap-12 items-center justify-items-center">
        <img v-for="logo in customerLogos.slice(5, 10)" :key="logo.id" :src="logo.src" :alt="logo.alt" class="partner-logo h-10">
      </div>
    </div>
  </section>

  <!-- Customer Success Stories -->
  <section class="bg-gray-50 pb-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-start">
        <!-- Left Column - Testimonials -->
        <div class="space-y-8">
          <div class="testimonial-card p-8 fade-in" v-for="testimonial in testimonials" :key="testimonial.id">
            <h3 class="text-xl font-bold text-blue-900 mb-4">{{ testimonial.title }}</h3>
            <p class="text-gray-700 mb-6 leading-relaxed">{{ testimonial.content }}</p>
            <div>
              <div class="font-semibold text-blue-900">{{ testimonial.name }}</div>
              <div class="text-sm text-gray-600">{{ testimonial.position }}</div>
            </div>
          </div>
        </div>
        
        <!-- Right Column - Header and Story -->
        <div class="space-y-8">
          <div>
            <h3 class="text-blue-600 text-lg font-semibold mb-2">Customer Success Stories</h3>
            <h2 class="text-4xl font-bold text-blue-900 mb-8">Take our word for it, take theirs too.</h2>
          </div>
          
          <div class="testimonial-card p-8">
            <h3 class="text-xl font-bold text-blue-900 mb-4">Fast and efficient</h3>
            <p class="text-gray-700 mb-6 leading-relaxed">
              Remis has been very handy. We have the privilege of being attended to promptly when we go to filling stations Remis is in partnership with. In times of scarcity, the customers using Remis like us are given priority treatment. Also, the fact that you generate a voucher on the platform and when taken to the station and inputted in the POS device, the value comes up makes it easy to use.
            </p>
            <div>
              <div class="font-semibold text-blue-900">Stephen Ibrahim</div>
              <div class="text-sm text-gray-600">Admin Partner, Qore</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Call to Action with Devices -->
  <section class="blue-gradient py-20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="bg-white rounded-3xl overflow-hidden grid grid-cols-1 lg:grid-cols-2 items-center">
        <div class="blue-gradient p-12 lg:p-16">
          <h2 class="text-4xl lg:text-5xl font-bold text-white mb-8 leading-tight">
            Take control of your Fleet & Fuel with Remis
          </h2>
        </div>
        <div class="p-8 lg:p-12 bg-gray-100">
          <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/47a9864a-d737-46a4-b214-74bb75e7f935.png" alt="Modern laptop and mobile devices displaying Remis dashboard interface with fuel management analytics and reporting features" class="w-full max-w-md mx-auto">
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const features = ref([
  {
    id: 1,
    title: 'Eliminate Cash Handling',
    description: 'Say goodbye to fraud and misuse. All transactions are digital and traceable.',
    icon: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/cbcd013e-98a1-45c7-8a59-5525ad578fbe.png',
    iconAlt: 'Digital wallet icon representing cashless fuel transactions'
  },
  {
    id: 2,
    title: 'Real-Time Monitoring',
    description: 'Track every litre, every driver, and every vehicle as it happens.',
    icon: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f4e911ea-5b8d-478f-8f52-1afa516666df.png',
    iconAlt: 'Real-time analytics chart icon showing live fuel monitoring dashboard'
  },
  {
    id: 3,
    title: 'Powerful Oversight',
    description: 'Assign fuel budgets, set limits, and review fuel purchase from every transaction on the dashboard.',
    icon: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ecb54ea1-e26b-440c-8aac-77cad082927a.png',
    iconAlt: 'Shield with checkmark icon representing security and oversight controls'
  },
  {
    id: 4,
    title: 'User-Friendly System',
    description: 'Easy-to-use fuel cards and vouchers that work seamlessly at authorized stations.',
    icon: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4028f5a1-7dcc-4798-bb22-afdabdb21984.png',
    iconAlt: 'User interface icon with simple design elements showing ease of use'
  },
  {
    id: 5,
    title: 'Instant Reconciliation',
    description: 'No more chasing reports. Get instant visibility into fuel usage by vehicle or department.',
    icon: 'https://placehold.co/32x32',
    iconAlt: 'Instant synchronization icon with circular arrows representing quick reconciliation'
  }
])

const testimonials = ref([
  {
    id: 1,
    title: 'Easy data collection',
    content: 'I have highlight using Remis but the major one is access to data for audit purposes. I can get data of 5 years in one day which is a plus for me.',
    name: 'Abiodun Oyewole',
    position: 'Transport and Admin, Jumia Nigeria'
  },
  {
    id: 2,
    title: 'Transparent transactions',
    content: 'Remis has made transactions so transparent. We can easily track records of purchase, even down to the time and driver that bought the fuel.',
    name: 'Omolara Oshoba',
    position: 'Administrative Officer, MISA'
  }
])

const customerLogos = ref([
  { id: 1, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4e01f645-e938-4ddd-8c58-4c52978c1b9a.png', alt: 'Jumia logo - orange shopping bag icon with company name for e-commerce platform' },
  { id: 2, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/fb676e05-59e3-4497-8031-f6cf9d020f52.png', alt: 'Qore logo - modern circular design with company name for tech company' },
  { id: 3, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/a9eeb1a4-238c-4ee7-aa0a-8057911bfa04.png', alt: 'Kova logo - stylized K with basketball design for sports organization' },
  { id: 4, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/dba51675-c4ba-4b40-80e6-64dc4c9a1b64.png', alt: 'Amber Energy Group logo - triangular mountain design in green representing energy company' },
  { id: 5, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/b3c88ace-2c19-4b13-b4bf-eaefae7c1df8.png', alt: 'VACC Technical Ltd logo - blue oval design with company name for technical services' },
  { id: 6, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ccf4994f-c2ff-468e-aa72-5ac6a34ec3f1.png', alt: 'WPAR logo - stylized W design in brown for business services company' },
  { id: 7, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/56888bdc-7c16-4319-bae9-728f7ed359a2.png', alt: 'Del-York Group logo - red circular emblem with company name for media group' },
  { id: 8, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/19a3c23a-e82f-4338-8fe9-17432d0abfb2.png', alt: 'Lifestores Healthcare logo - green medical cross with company name for pharmacy chain' },
  { id: 9, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/b2906ccc-5286-4879-8dac-ac35c57f9b96.png', alt: 'Deologistics logo - purple geometric design with company name for logistics company' },
  { id: 10, src: 'https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/a26a3a11-0c9f-4730-b768-7c9eecb7e33b.png', alt: 'Dreamworks logo - modern text design with tagline for creative services company' }
])

onMounted(() => {
  observeElements()
})

const observeElements = () => {
  const observerOptions = {
    threshold: 0.1,
    rootMargin: '0px 0px -50px 0px'
  }
  
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible')
      }
    })
  }, observerOptions)
  
  document.querySelectorAll('.fade-in').forEach(el => {
    observer.observe(el)
  })
}
</script>

<style scoped>
/* Component-specific styles if needed */
</style>
