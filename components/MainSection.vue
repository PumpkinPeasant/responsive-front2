<script setup lang="ts">

</script>

<template>
  <section class="main-section">
    <h1 class="text-neutral-100 text-uppercase">We are creatives</h1>
  </section>
</template>

<style scoped>
.main-section{
  height: 100dvh;
  background-image: url("/assets/images/desktop/image-header.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

@media (max-width: 50em) /* 800px */ {
  .main-section{
    background-image: url("/assets/images/mobile/image-header.jpg");
  }
}
</style>