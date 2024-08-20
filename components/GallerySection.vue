<script setup lang="ts">
import ConeImg from '~/assets/images/desktop/image-gallery-cone.jpg'
import MilkBottlesImg from '~/assets/images/desktop/image-gallery-milkbottles.jpg'
import OrangeImg from '~/assets/images/desktop/image-gallery-orange.jpg'
import SugarCubesImg from '~/assets/images/desktop/image-gallery-sugarcubes.jpg'

</script>

<template>
  <section>
    <div class="even-columns">
      <img :src="MilkBottlesImg" alt="Milk bottles">
      <img :src="OrangeImg" alt="Orange">
      <img :src="ConeImg" alt="Cone">
      <img :src="SugarCubesImg" alt="Sugar cubes">
    </div>
  </section>
</template>

<style scoped>
* {
  --even-columns-gap: 0;
}
</style>