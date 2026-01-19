<script setup>
import greenPublicLogo from '@/assets/images/green-public.png';
</script>

<template>
  <section id="section-header">
    <div class="container header-wrapper">
      <header class="site-header">
        <div class="logo">
          <img
            :src="greenPublicLogo"
            alt="Green Public Logo"
            class="logo-img"
          />
        </div>

        <div class="language-selector">
          <span class="lang-text">AZ</span>
        </div>
      </header>
    </div>
  </section>
</template>
