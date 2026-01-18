<template>
  <div class="rounded-full h-16 w-16 bg-gray-300 flex items-center justify-center">
    <img :src="src" alt="Avatar" class="rounded-full h-14 w-14 object-cover">
  </div>
</template>

<script setup>
defineProps({
  src: String,
});
</script>