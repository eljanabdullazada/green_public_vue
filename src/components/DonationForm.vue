<template>
  <div class="backdrop-blur-xl bg-white/10 border border-white/10 rounded-2xl p-10 shadow-xl">
    <form class="grid grid-cols-2 gap-6">

      <input placeholder="First Name" class="form-input bg-white text-black rounded-lg px-4 py-3 shadow-inner" />
      <input placeholder="Last Name" class="form-input bg-white text-black rounded-lg px-4 py-3 shadow-inner" />

      <input placeholder="Email" class="form-input bg-white text-black rounded-lg px-4 py-3 shadow-inner" />
      <input placeholder="Company Name" class="form-input bg-white text-black rounded-lg px-4 py-3 shadow-inner" />

      <input type="number" placeholder="Number of Trees" class="form-input bg-white text-black rounded-lg px-4 py-3 shadow-inner" />

      <select class="form-select bg-white text-black rounded-lg px-4 py-3 shadow-inner">
        <option>Olive Tree – 25 ₼</option>
      </select>

      <select class="form-select bg-white text-black rounded-lg px-4 py-3 shadow-inner col-span-2">
        <option>Tree donation</option>
      </select>

      <select class="form-select bg-white text-black rounded-lg px-4 py-3 shadow-inner col-span-2">
        <option>Absheron – Khizi Economic Region</option>
      </select>

      <textarea placeholder="For whom or for what"
        class="form-textarea bg-white text-black rounded-lg px-4 py-3 shadow-inner col-span-2 h-28 resize-none"></textarea>

      <div class="col-span-2 flex justify-end">
        <button type="button" class="bg-[#1c4b2b] hover:bg-[#143821] px-10 py-3 rounded-xl font-medium">
          Donate
        </button>
      </div>
    </form>
  </div>
</template>
