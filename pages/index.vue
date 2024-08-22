<script setup lang="ts">
import GallerySection from "~/components/GallerySection.vue";
</script>

<template>
  <div>
    <app-header/>
    <main>
      <main-section  class="container"/>
      <about-section/>
      <reviews-section class="container"/>
      <gallery-section/>
    </main>
    <app-footer class="container"/>
  </div>
</template>

<style scoped>

</style>