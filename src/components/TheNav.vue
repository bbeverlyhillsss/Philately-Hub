<template>
  <nav class="flex flex-wrap gap-10 items-center">
    <NavItem
      v-for="(icon, page) in navItems"
      :key="page"
      v-bind:href="`#${page}`"
      :class="{ 'pointer-events-none': page == currentPage }"
      @click="currentPage = page"
    >
      <component :is="icon" class="size-5" /> {{ page }}
    </NavItem>
  </nav>
</template>

<script setup>
import { ref } from 'vue'
import { HomeIcon, RectangleStackIcon, UserIcon } from '@heroicons/vue/24/solid'
import { PAGE_HOMEPAGE, PAGE_CATALOG, PAGE_PROFILE } from '@/constants.js'
import NavItem from '@/components/NavItem.vue'

const navItems = {
  [PAGE_HOMEPAGE]: HomeIcon,
  [PAGE_CATALOG]: RectangleStackIcon,
  [PAGE_PROFILE]: UserIcon,
}
const currentPage = ref(normalizePageHash())

function normalizePageHash() {
  const hash = window.location.hash.slice(1)
  if (Object.keys(navItems).includes(hash)) {
    return hash
  } 
  window.location.hash = PAGE_HOMEPAGE
  return PAGE_HOMEPAGE
}
</script>
