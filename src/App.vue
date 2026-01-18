<template>
  <component :is="currentView" />
</template>

<script setup>
import { ref, computed } from 'vue'
import DonationView from './views/DonationView.vue'
import CertificateView from './views/CertificateView.vue'

const showDonate = ref(true)
window.swap = () => showDonate.value = !showDonate.value // debug swap

const currentView = computed(() =>
  showDonate.value ? DonationView : CertificateView
)
</script>
