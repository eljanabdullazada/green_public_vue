<template>
  <div class="min-h-screen bg-gradient-to-br from-[#003b27] via-[#006040] to-[#0b8f65] text-white overflow-hidden">

    <HeaderBar />

    <main class="container mx-auto px-6 text-center mt-20">
      <h1 class="text-6xl font-semibold tracking-tight">Donate Trees</h1>
      <p class="mt-4 text-white/80 max-w-2xl mx-auto leading-relaxed">
        Our services support ESG performance and carbon management through reliable data and practical tools.
      </p>

      <div class="flex flex-col lg:flex-row justify-center items-start gap-14 mt-16">
        <div class="w-full lg:w-[60%]">
          <AzerbaijanMap />
        </div>
        <div class="w-full lg:w-[40%]">
          <DonationForm />
        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
import HeaderBar from '../components/HeaderBar.vue'
import AzerbaijanMap from '../components/AzerbaijanMap.vue'
import DonationForm from '../components/DonationForm.vue'
</script>
