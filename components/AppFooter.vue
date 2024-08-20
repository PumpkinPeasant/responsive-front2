<script setup lang="ts">
import Logo from '~/assets/images/logo.svg'
import Facebook from "~/assets/icons/icon-facebook.svg";
import Twitter from "~/assets/icons/icon-twitter.svg";
import Pinterest from "~/assets/icons/icon-pinterest.svg";
import Instagram from "~/assets/icons/icon-instagram.svg";

const links = [
  {
    label: 'Facebook',
    icon: Facebook,
    href: '#',
  },
  {
    label: 'Twitter',
    icon: Twitter,
    href: '#',
  },
  {
    label: 'Pinterest',
    icon: Pinterest,
    href: '#',
  },
  {
    label: 'Instagram',
    icon: Instagram,
    href: '#',
  },
]
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
  <footer class="primary-footer">
    <logo :fontControlled="false" filled style="width: 10rem"/>
    <nav aria-label="Secondary"
         class="secondary-navigation">
      <ul class="nav-list" role="list">
        <li v-for="(item, index) in navItems" :key="index">
          <a :href="item.href">{{ item.title }}</a>
        </li>
      </ul>
    </nav>

    <ul class="social-media" role="list" aria-label="Social links">
      <li v-for="(link, index) in links" :key="index">
        <a :aria-label="link.label" :href="link.href">
          <component :is="link.icon"/>
        </a>
      </li>
    </ul>
  </footer>
</template>

<style scoped>
.primary-footer {
  background-color: var(--clr-green-100);
}
</style>