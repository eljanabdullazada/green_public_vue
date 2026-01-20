<script setup>
import { ref, onMounted, onUnmounted } from 'vue';
import ArrowIcon from './icons/ArrowIcon.vue';

// State for Tree Type Dropdown
const isTreeTypeOpen = ref(false);
const selectedTreeType = ref('Olive Tree - 25 ₼');
const treeTypeOptions = ref(['Olive Tree - 25 ₼', 'Pine Tree - 30 ₼', 'Oak Tree - 35 ₼']);

// State for Donation Type Dropdown
const isDonationTypeOpen = ref(false);
const selectedDonationType = ref('Tree donation');
const donationTypeOptions = ref(['Tree donation', 'Carbon offset', 'General support']);

// State for Planting Zone Dropdown
const isPlantingZoneOpen = ref(false);
const selectedPlantingZone = ref('Absheron - Khizi Economic Region');
const plantingZoneOptions = ref(['Absheron - Khizi Economic Region', 'Ganja-Dashkasan', 'Shaki-Zagatala']);

const closeAllDropdowns = () => {
  isTreeTypeOpen.value = false;
  isDonationTypeOpen.value = false;
  isPlantingZoneOpen.value = false;
};

const toggleDropdown = (type) => {
  const wasOpen = {
    tree: isTreeTypeOpen.value,
    donation: isDonationTypeOpen.value,
    zone: isPlantingZoneOpen.value
  }[type];

  closeAllDropdowns();

  if (!wasOpen) {
    if (type === 'tree') isTreeTypeOpen.value = true;
    if (type === 'donation') isDonationTypeOpen.value = true;
    if (type === 'zone') isPlantingZoneOpen.value = true;
  }
};

const selectOption = (type, option) => {
  if (type === 'tree') selectedTreeType.value = option;
  if (type === 'donation') selectedDonationType.value = option;
  if (type === 'zone') selectedPlantingZone.value = option;
  closeAllDropdowns();
};

const handleClickOutside = (event) => {
  if (!event.target.closest('.dropdown-wrapper')) {
    closeAllDropdowns();
  }
};

onMounted(() => {
  document.addEventListener('click', handleClickOutside);
});

onUnmounted(() => {
  document.removeEventListener('click', handleClickOutside);
});
</script>

<template>
  <div class="donation-form">
    <div class="form-row">
      <div class="form-group">
        <label>First Name</label>
        <div class="input-wrapper">
          <input type="text" value="Name" />
        </div>
      </div>
      <div class="form-group">
        <label>Last Name</label>
        <div class="input-wrapper">
          <input type="text" value="Surname" />
        </div>
      </div>
    </div>

    <div class="form-row">
      <div class="form-group">
        <label>Email adress</label>
        <div class="input-wrapper">
          <input type="email" value="@gmail.com" />
        </div>
      </div>
      <div class="form-group">
        <label>Company Name</label>
        <div class="input-wrapper">
          <input type="text" value="Green Public" />
        </div>
      </div>
    </div>

    <div class="form-row">
      <div class="form-group">
        <label>Number of Trees</label>
        <div class="input-wrapper">
          <input type="number" value="1" min="1" step="1" />
        </div>
      </div>
      <div class="form-group dropdown-wrapper">
        <label>Tree Type</label>
        <div class="input-wrapper dropdown" @click="toggleDropdown('tree')">
          <span>{{ selectedTreeType }}</span>
          <ArrowIcon :class="{ 'rotate-180': isTreeTypeOpen }" />
        </div>
        <ul v-if="isTreeTypeOpen" class="dropdown-options">
          <li v-for="option in treeTypeOptions" :key="option" @click="selectOption('tree', option)">
            {{ option }}
          </li>
        </ul>
      </div>
    </div>

    <div class="form-group full-width dropdown-wrapper">
      <label>Select your donation type</label>
      <div class="input-wrapper dropdown" @click="toggleDropdown('donation')">
        <span>{{ selectedDonationType }}</span>
        <ArrowIcon :class="{ 'rotate-180': isDonationTypeOpen }" />
      </div>
      <ul v-if="isDonationTypeOpen" class="dropdown-options">
        <li v-for="option in donationTypeOptions" :key="option" @click="selectOption('donation', option)">
          {{ option }}
        </li>
      </ul>
    </div>

    <div class="form-group full-width dropdown-wrapper">
      <label>Planting Zone</label>
      <div class="input-wrapper dropdown" @click="toggleDropdown('zone')">
        <span>{{ selectedPlantingZone }}</span>
        <ArrowIcon :class="{ 'rotate-180': isPlantingZoneOpen }" />
      </div>
       <ul v-if="isPlantingZoneOpen" class="dropdown-options">
        <li v-for="option in plantingZoneOptions" :key="option" @click="selectOption('zone', option)">
          {{ option }}
        </li>
      </ul>
    </div>

    <div class="form-group full-width">
      <label>Donation For Whom or For What</label>
      <div class="input-wrapper textarea-like">
        <textarea placeholder=""></textarea>
      </div>
    </div>

    <button class="btn-donate">Donate</button>
  </div>
</template>