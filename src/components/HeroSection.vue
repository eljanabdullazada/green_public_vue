<template>
  <section id="section-hero">
    <div class="container hero-container">
      <!-- Background Elements -->
      

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
          <img src="../assets/images/azerbaijan.svg" alt="Azerbaijan Map" class="hero-map-image" />

          <!-- Donation Form -->
          <DonationForm />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import DonationForm from './DonationForm.vue';
</script>