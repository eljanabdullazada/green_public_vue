<template>
  <header class="w-full mx-auto mt-6 bg-white/10 backdrop-blur-xl rounded-3xl shadow-lg">
    <nav class="px-10 py-4 flex justify-between items-center">
      <div class="flex items-center space-x-2">
        <img src="/vite.svg" class="h-8 w-8" />
        <span class="font-semibold text-xl">Green Public</span>
      </div>
      <div class="hidden md:flex space-x-8 text-white/90 font-medium">
        <a href="#" class="nav-link">Home</a>
        <a href="#" class="nav-link">About us</a>
        <a href="#" class="nav-link">Donation</a>
      </div>
      <button class="border border-white/50 rounded-full px-4 py-1 text-sm">AZ</button>
    </nav>
  </header>
</template>

<style scoped>
.nav-link {
  @apply hover:text-green-300;
}
</style>
