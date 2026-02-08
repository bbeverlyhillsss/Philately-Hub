<template>
  <div class="min-h-screen bg-linear-to-b from-[#94B0DA] to-[#CBD5E1] text-slate-900 font-sans">
    <TheHeader></TheHeader> 
    <TheMain></TheMain>
    <TheFooter></TheFooter>
  </div>
</template>

<script setup>
import TheHeader from '@/components/TheHeader.vue'
import TheMain from '@/components/TheMain.vue'
import TheFooter from '@/components/TheFooter.vue'
</script>

<style>
body {
  margin: 0px;
  padding: 0px;
}
</style>
