<script setup lang="ts">
import EmilyImg from '~/assets/images/image-emily.jpg'
import JennieImg from '~/assets/images/image-jennie.jpg'
import ThomasImg from '~/assets/images/image-thomas.jpg'

const cards = [
  {
    avatar: EmilyImg,
    text: 'We put our trust in Sunnyside and they\n' +
        'delivered, making sure our needs were\n' +
        'met and deadlines were always hit.',
    name: 'Emily R.',
    position: 'Marketing Director',
  },
  {
    avatar: ThomasImg,
    text: 'Sunnyside enthusiasm coupled with\n' +
        'their keen interest in our brand\'s success\n' +
        'made it a satisfying and enjoyable\n' +
        'experience.',
    name: 'Thomas S.',
    position: 'Chief Operating Officer',
  },
  {
    avatar: JennieImg,
    text: 'Incredible end result! Our sales increased\n' +
        'over 400% when we worked with\n' +
        'Sunnyside. Highly recommended!',
    name: 'Jennie F.',
    position: 'Business Owner',
  },
]
</script>

<template>
  <section>
    <h2 class="text-uppercase">Client testimonials</h2>
    <div class="even-columns">
      <div v-for="(card, index) in cards" :key="index">
        <img :src="card.avatar" alt="">
        <p>{{ card.text }}</p>
        <div>
          <p class="ff-primary text-primary-800 fw-bold">{{ card.name }}</p>
          <p>{{ card.position }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>

</style>