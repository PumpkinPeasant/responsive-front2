<script setup lang="ts">
import ArrowIcon from "~/assets/icons/icon-arrow-down.svg";
</script>

<template>
  <section class="main-section">
    <h1 class="text-neutral-100 text-uppercase fs-primary-heading fw-bold">We are creatives</h1>
    <arrow-icon class="arrow" :fontControlled="false" filled style="width: 2rem"/>
  </section>
</template>

<style scoped>
.main-section {
  height: 100dvh;
  background-image: url("/assets/images/desktop/image-header.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

h1 {
  text-align: center;
}

.arrow {
  cursor: pointer;
}

@media (max-width: 50em) /* 800px */ {
  .main-section {
    background-image: url("/assets/images/mobile/image-header.jpg");
  }
}
</style>