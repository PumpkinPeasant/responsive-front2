<script setup lang="ts">
import Logo from '~/assets/images/logo.svg'

const navItems = [
  {
    title: 'About',
    href: '#',
  },
  {
    title: 'Services',
    href: '#',
  },
  {
    title: 'Projects',
    href: '#',
  },
]
</script>

<template>
  <header class="primary-header">
    <logo :fontControlled="false" filled style="width: 10rem"/>
    <div>
      <nav aria-label="Primary"
           class="primary-navigation"
           id="primary-navigation">
        <ul class="text-neutral-100 | nav-list" role="list">
          <li v-for="(item, index) in navItems" :key="index">
            <a :href="item.href">{{ item.title }}</a>
          </li>
        </ul>
      </nav>
      <button class="text-uppercase ff-primary">Contact</button>
    </div>
  </header>
</template>

<style scoped>
.primary-header {
  position: fixed;
  width: 100%;
  z-index: 2;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>