<template>
  <section id="section-hero">
    <!-- Background Elements -->
    <img
      src="../assets/images/header-form-background.png"
      alt="background-element"
      class="background-element"
    />
    <div class="container hero-container">
      <div class="hero-content">
        <div class="hero-titles">
          <h1 class="main-title">Donate Trees</h1>
          <p class="subtitle">
            Our services support ESG performance and carbon management through
            reliable data and practical tools.
          </p>
        </div>

        <div class="hero-layout-container">
          <div class="hero-left-column">
            <div class="hero-map-wrapper">
              <img
                src="../assets/images/azerbaijan.svg"
                alt="Azerbaijan Map"
                class="hero-map-image"
              />
            </div>

            <div class="hero-logos-wrapper">
              <img
                src="../assets/images/green-public.svg"
                alt="Green Public Logo"
                class="hero-logo-image"
              />
              <img
                src="../assets/images/eco-logo.svg"
                alt="Eco Logo"
                class="hero-logo-image"
              />
            </div>
          </div>
          <!-- Donation Form -->
          <DonationForm />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import DonationForm from "./DonationForm.vue";
</script>

<style scoped>
#section-hero {
  position: relative;
}

.background-element {
  position: absolute;
  bottom: 40px;
  right: 0;
  z-index: 0;
  filter: blur(0px);
  transform: scale(0.9);
  transform-origin: bottom right;
}

.hero-container {
  position: relative;
  z-index: 1;
}
</style>
