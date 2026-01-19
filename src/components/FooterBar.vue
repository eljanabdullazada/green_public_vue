<script setup>
import LinkedInIcon from './icons/LinkedInIcon.vue';
import InstagramIcon from './icons/InstagramIcon.vue';
import TwitterIcon from './icons/TwitterIcon.vue';
import YouTubeIcon from './icons/YouTubeIcon.vue';
</script>

<template>
  <section id="section-footer">
    <footer class="site-footer">
      <div class="container">
        <div class="footer-top">
          <div class="footer-logo-group">
            <div class="footer-logo">
              <img
                :src="assets/images/about"
                alt="Logo"
              />
              <img
                src="https://via.placeholder.com/150x62.png?text=Eco+Logo"
                alt="Eco Logo"
              />
            </div>
          </div>

          <div class="footer-info">
            <div class="info-item">
              <span class="info-label">Location</span>
              <p class="info-text">Baku, Azerbaijan, at Cefer Cabbarlı Street</p>
            </div>
            <div class="info-item">
              <span class="info-label">Email</span>
              <p class="info-text">greenpublic@gmail.com</p>
            </div>
          </div>

          <div class="footer-socials">
            <a href="#" class="social-icon"><LinkedInIcon /></a>
            <a href="#" class="social-icon"><InstagramIcon /></a>
            <a href="#" class="social-icon"><TwitterIcon /></a>
            <a href="#" class="social-icon"><YouTubeIcon /></a>
          </div>
        </div>

        <div class="footer-bottom">
          <p>GreenPublic© 2025 All Rights Reserved</p>
          <div class="footer-links">
            <a href="#">Privacy Policy</a>
            <span>|</span>
            <a href="#">Terms & Conditions</a>
          </div>
        </div>
      </div>
    </footer>
  </section>
</template>
