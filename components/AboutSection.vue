<script setup lang="ts">
import TransformImg from '~/assets/images/desktop/image-transform.jpg'
import StandOutImg from '~/assets/images/desktop/image-stand-out.jpg'
import GraphicDesignImg from '~/assets/images/desktop/image-graphic-design.jpg'
import PhotographyImg from '~/assets/images/desktop/image-photography.jpg'

</script>

<template>
  <section>
    <div class="even-columns">
      <div>
        <h2>
          Transform your brand
        </h2>
        <p>
          We are a full-service creative agency specializing in
          helping brands grow fast. Engage your clients through
          compelling visuals that do most of the marketing for you.
        </p>
        <button>LEARN MORE</button>
      </div>
      <div>
        <img :src="TransformImg" alt="Egg image">
      </div>
    </div>
    <div class="even-columns">
      <img :src="StandOutImg" alt="Egg image">
      <div>
        <h2>Stand out to the right
          audience</h2>
        <p>Using a collaborative formula of designers, researchers,
          photographers, videographers, and copywriters, we'll
          build and extend your brand in digital places.</p>
        <button>LEARN MORE</button>
      </div>
    </div>
    <div class="even-columns">
      <div class="graphic-design">
        <img :src="GraphicDesignImg" alt="Orange">
        <div class="card-content">
          <h2>
            Graphic Design
          </h2>
          <p>
            Great design makes you memorable. We deliver
            artwork that underscores your brand message
            and captures potential clients' attention.
          </p>
        </div>
      </div>
      <div class="photography">
        <img :src="PhotographyImg" alt="Orange">
        <div class="card-content">
          <h2>
            Photography
          </h2>
          <p>
            Increase your credibility by getting the most
            stunning, high-quality photos that improve your
            business image.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
* {
  --even-columns-gap: 0;
}

h2 {
  font-family: var(--ff-heading);
  font-weight: var(--fw-bold);
}

p {
  font-family: var(--ff-body);
  font-weight: var(--fw-regular);
}

img {
  width: 100%;
}

.graphic-design, .photography {
  position: relative;
}

.card-content {
  position: absolute;
  top: 50%;
}
</style>