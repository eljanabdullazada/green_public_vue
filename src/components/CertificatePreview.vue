<script setup>
import certificate from '@/assets/images/certificate.png';
</script>

<template>
  <section id="certificate-preview">
    <div class="certificate-container">
      <div class="certificate-content">
        <!-- Left Column: Text Content -->
        <div class="text-column">
          <div class="badge">
            <div class="badge-dot"></div>
            <span class="badge-text">Certificate</span>
          </div>

          <div class="text-wrapper">
            <h2 class="main-title">Your Certificate Preview</h2>
            <p class="description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut et massa
              mi. Aliquam in hendrerit urnaellentesque si
            </p>
          </div>
        </div>

        <!-- Right Column: Image -->
        <div class="image-column">
          <img
            :src="certificate"
            alt="Certificate Preview"
            class="certificate-image"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Section Container */
#certificate-preview {
  width: 100%;
  display: flex;
  justify-content: center;
  background-color: #fff;
}

.certificate-container {
  width: 100%;
  max-width: 1440px; /* Root frame width */
  margin: 0 auto;
}

/* Main Flex Layout */
.certificate-content {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-start; /* style_1 */
  gap: 80px; /* style_1 */
  padding: 60px 80px; /* style_1 */
}

/* Left Column */
.text-column {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  gap: 8px; /* style_2 */
  width: 100%;
  max-width: 547px; /* style_2 */
}

/* Badge Component */
.badge {
  background-color: #f2f5f3; /* style_3 */
  display: inline-flex;
  flex-direction: row;
  align-items: center;
  gap: 4px; /* style_3 */
  padding: 2px 8px; /* style_3 */
  border-radius: 4px; /* style_3 */
  box-shadow: 0px 4px 8px 0px rgba(0, 0, 0, 0.1); /* style_3 */
  margin-bottom: 8px; /* Visual spacing adjustment */
}

.badge-dot {
  width: 8px;
  height: 8px;
  background-color: #0be055; /* style_4 */
  border-radius: 100px; /* style_4 */
}

.badge-text {
  color: #6e726e; /* style_5 */
  font-size: 12px; /* Estimated from height 20px */
  font-weight: 500;
  line-height: 1.5;
}

/* Text Content */
.text-wrapper {
  display: flex;
  flex-direction: column;
  gap: 8px; /* style_6 */
  width: 100%;
}

.main-title {
  margin: 0;
  color: #3b3d3b; /* style_7 */
  font-size: 36px; /* Estimated from height 48px */
  font-weight: 700;
  line-height: 1.2;
}

.description {
  margin: 0;
  color: #aaaaaa; /* style_8 */
  font-size: 16px; /* Estimated from height 52px */
  font-weight: 400;
  line-height: 1.6;
}

/* Right Column */
.image-column {
  flex: 1;
  display: flex;
  justify-content: flex-start;
  max-width: 651px;
}

.certificate-image {
  width: 100%;
  height: auto;
  border: 0.5px solid #0be055; /* style_9 */
  border-radius: 10px; /* style_9 rounded */
  box-shadow: 0px 0px 14px 14px rgba(191, 255, 185, 0.2); /* style_9 */
  object-fit: cover;
}

/* Responsive Design */
 @media (max-width: 1024px) {
  .certificate-content {
    flex-direction: column;
    align-items: center;
    gap: 40px;
    padding: 40px 20px;
  }

  .text-column {
    max-width: 100%;
    align-items: center;
    text-align: center;
  }

  .image-column {
    width: 100%;
    justify-content: center;
  }
}

 @media (max-width: 480px) {
  .main-title {
    font-size: 28px;
  }

  .description {
    font-size: 14px;
  }
}
</style>
