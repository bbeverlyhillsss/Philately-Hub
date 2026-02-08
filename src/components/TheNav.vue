<template>
  <nav class="flex flex-wrap gap-10 items-center">
    <li
      class="flex items-center gap-2 px-6 py-2 rounded-full bg-slate-800 text-white font-black tracking-tight transition-all duration-300 hover:scale-110 hover:bg-slate-700 hover:shadow-xl cursor-pointer active:scale-95"
    >
      <HomeIcon class="size-5" /><span> Home Page</span>
    </li>
    <li
      class="flex items-center gap-2 px-6 py-2 rounded-full bg-slate-800 text-white font-black tracking-tight transition-all duration-300 hover:scale-110 hover:bg-slate-700 hover:shadow-xl cursor-pointer active:scale-95"
    >
      <RectangleStackIcon class="size-5" /><span> Catalog</span>
    </li>
    <li
      class="flex items-center gap-2 px-6 py-2 rounded-full bg-slate-800 text-white font-black tracking-tight transition-all duration-300 hover:scale-110 hover:bg-slate-700 hover:shadow-xl cursor-pointer active:scale-95"
    >
      <UserIcon class="size-5" /><span> Profile</span>
    </li>
  </nav>
</template>

<script setup>
import { HomeIcon, RectangleStackIcon, UserIcon } from '@heroicons/vue/24/solid'
</script>
