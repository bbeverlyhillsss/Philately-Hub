<template>
  <main class="max-w-7xl mx-auto px-6 py-16 md:py-24">
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
      <div class="space-y-8">
        <MainSectionText></MainSectionText>
        <Search></Search>
      </div>
    </div>
  </main>
</template>

<script setup>
import MainSectionText from './MainSectionText.vue'
import Search from './Search.vue'
</script>
