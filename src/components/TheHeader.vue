<template>
  <header class="p-4 border-b border-white/0">
    <div class="max-w-7xl mx-auto">
      <ul class="flex items-center justify-between gap-4">
        <li class="shrink-0">
          <TheLogo></TheLogo>
        </li>
        <TheNav></TheNav>
      </ul>
    </div>
  </header>
</template>

<script setup>
import TheLogo from './TheLogo.vue'
import TheNav from './TheNav.vue'
</script>
