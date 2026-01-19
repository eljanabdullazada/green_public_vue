<template>
  <HeaderBar />
  <main>
    <HeroSection />
    <section id="section-certificate">
      <div class="container certificate-container">
        <div class="cert-content">
          <div class="tag-pill">
            <div class="dot"></div>
            <span>Certificate</span>
          </div>
          <h2 class="section-title">Your Certificate Preview</h2>
          <p class="section-desc">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut et massa mi.
            Aliquam in hendrerit urnaellentesque si
          </p>
        </div>
        <div class="cert-image-wrapper">
          <CertificatePreview />
        </div>
      </div>
    </section>
    <AboutSection />
  </main>
  <FooterBar />
</template>

<script setup>
import HeaderBar from './components/HeaderBar.vue'
import HeroSection from './components/HeroSection.vue'
import CertificatePreview from './components/CertificatePreview.vue'
import AboutSection from './components/AboutSection.vue'
import FooterBar from './components/FooterBar.vue'
</script>
