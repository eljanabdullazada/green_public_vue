<template>
  <section id="section-hero">
    <img
      src="../assets/images/left-top-background-mobile.svg"
      alt="ellipse-left-top"
      class="ellipse-left-top"
    />
    <img
      src="../assets/images/ellipse-right-bottom.png"
      alt="ellipse-right-bottom"
      class="ellipse-right-bottom"
    />
    <!-- Background Elements header-form-background.png-->
    <img
      src="../assets/images/bg.png"
      alt="background-element"
      class="background-element"
    />
    <div class="hero-container">
      <div class="hero-content">
        <div class="hero-titles">
          <h1 class="main-title">Donate Trees</h1>
          <p class="subtitle">
            Our services support ESG performance and carbon management 
            through reliable data and practical tools.
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
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: 0;
}

.hero-container {
  position: relative;
  z-index: 1;
}

.ellipse-left-top {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 2;
  /* mix-blend-mode: overlay; */
  filter: blur(120px);
  rotate: 60deg;
}

.ellipse-right-bottom {
  position: absolute;
  bottom: 0;
  right: 0;
  z-index: 1;
  mix-blend-mode: overlay;
  filter: blur(50px);
  opacity: 0.6;
}

@media (max-width: 1024px) {
  .ellipse-left-top {
    width: 120%;
    top: -10%;
    left: -10%;

    filter: blur(90px);
    rotate: 30deg;
    z-index: 1;
  }
}

@media (max-width: 768px) {
  .ellipse-right-bottom {
    display: none;
  }

 .ellipse-left-top {
    position: absolute;
    /* top: -20%;
    left: -20%; */
    width: 140%;
    height: auto;

    z-index: 0;

    filter: blur(60px);     
    rotate: 0deg;            
    /* opacity: 0.9; */
  }

}
</style>
