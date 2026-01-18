<template>
  <div class="bg-white">
    <div class="container mx-auto px-6 py-16 text-center">
      <span class="text-green-500 text-sm font-medium">● Certificate</span>
      <h1 class="text-4xl font-semibold mt-2">Your Certificate Preview</h1>
      <p class="text-gray-500 mt-4 max-w-2xl mx-auto leading-relaxed">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      </p>

      <div class="flex justify-center items-center gap-10 mt-14">
        <div class="relative w-1/2">
          <FloatingAvatar class="absolute top-28 left-20" />
          <FloatingAvatar class="absolute top-60 left-60" />
        </div>
        <div class="w-1/2">
          <CertificatePreview />
        </div>
      </div>
    </div>

    <MainFooter />
  </div>
</template>

<script setup>
import FloatingAvatar from '../components/FloatingAvatar.vue'
import CertificatePreview from '../components/CertificatePreview.vue'
// import MainFooter from '../components/footer/MainFooter.vue'w
</script>
