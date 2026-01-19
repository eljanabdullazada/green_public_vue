<template>
  <section id="section-hero">
    <div class="container hero-container">
      <!-- Background Elements -->
      <div class="hero-bg">
        <div class="bg-blur blur-1"></div>
        <div class="bg-blur blur-2"></div>
        <div class="bg-blur blur-3"></div>
      </div>

      <div class="hero-content">
        <div class="hero-titles">
          <h1 class="main-title">Donate Trees</h1>
          <p class="subtitle">
            Our services support ESG performance and carbon management through
            reliable data and practical tools.
          </p>
        </div>

        <div class="hero-main-row">
          <!-- Map Visualization -->
          <AzerbaijanMap />

          <!-- Donation Form -->
          <DonationForm />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import AzerbaijanMap from './AzerbaijanMap.vue';
import DonationForm from './DonationForm.vue';
</script>
