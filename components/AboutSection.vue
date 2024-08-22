<script setup lang="ts">
import TransformImg from '~/assets/images/desktop/image-transform.jpg'
import StandOutImg from '~/assets/images/desktop/image-stand-out.jpg'
import GraphicDesignImg from '~/assets/images/desktop/image-graphic-design.jpg'
import PhotographyImg from '~/assets/images/desktop/image-photography.jpg'

</script>

<template>
  <section>
    <div class="even-columns">
      <div class="section-block | flow">
        <h2 class="text-primary-800 fs-secondary-heading">
          Transform your brand
        </h2>
        <p class="text-neutral-300">
          We are a full-service creative agency specializing in
          helping brands grow fast. Engage your clients through
          compelling visuals that do most of the marketing for you.
        </p>
        <button
            class="button | text-uppercase text-primary-800 ff-primary"
            style="--background-color: var(--clr-yellow-300)">
          Learn more
        </button>
      </div>
      <div>
        <img :src="TransformImg" alt="Egg image">
      </div>
    </div>
    <div class="even-columns">
      <img :src="StandOutImg" alt="Egg image">
      <div class="section-block | flow">
        <h2 class="text-primary-800 fs-secondary-heading">Stand out to the right audience</h2>
        <p class="text-neutral-300">Using a collaborative formula of designers, researchers,
          photographers, videographers, and copywriters, we'll
          build and extend your brand in digital places.</p>
        <button
            class="button | text-uppercase text-primary-800 ff-primary"
            style="--background-color: var(--clr-orange-200)">
          Learn more
        </button>
      </div>
    </div>
    <div class="even-columns">
      <div class="graphic-design">
        <img :src="GraphicDesignImg" alt="Orange">
        <div class="card-content | flow">
          <h2 class="text-green-400 fs-third-heading">
            Graphic Design
          </h2>
          <p class="text-green-400">
            Great design makes you memorable. We deliver
            artwork that underscores your brand message
            and captures potential clients' attention.
          </p>
        </div>
      </div>
      <div class="photography">
        <img :src="PhotographyImg" alt="Orange">
        <div class="card-content | flow">
          <h2 class="text-cyan-400 fs-third-heading">
            Photography
          </h2>
          <p class="text-cyan-400">
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

.section-block {
  --padding: 1rem;
  align-self: center;
  justify-self: end;
  width: min(var(--max-width) / 2, 100% - var(--padding) * 2);
}

.section-block:nth-child(odd) {
  margin-left: auto;
}

.section-block:nth-child(even) {
  margin-right: auto;
}

.graphic-design, .photography {
  position: relative;
}

.card-content {
  text-align: center;
  position: absolute;
  top: 50%;
}

.button {
  background: transparent;
  border: unset;
  position: relative;
  font-weight: var(--fw-bold);
}

.button::before {
  z-index: -1;
  content: '';
  position: absolute;
  height: 0.6em;
  bottom: 0;
  left: -10px;
  right: -10px;
  border-radius: 5px;
  background: var(--background-color);
  opacity: 0.3;
}

.button:hover::before,
.button:focus-visible::before {
  opacity: 1;
}

</style>