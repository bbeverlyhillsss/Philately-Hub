<template>
  <form action="/search" class="w-full max-w-xl">
    <div
      class="flex items-center bg-white/40 backdrop-blur-xl rounded-full p-2 border border-white/50 shadow-2xl transition-all duration-500 focus-within:scale-105 focus-within:bg-white/60"
    >
      <input
        type="search"
        name="q"
        placeholder="Search stamps..."
        class="flex-1 bg-transparent border-none outline-none focus:ring-0 px-6 py-3 text-slate-800 placeholder:text-slate-500 font-medium text-lg w-full"
      />

      <button
        type="submit"
        class="flex items-center gap-2 bg-slate-800 text-white px-8 py-3 rounded-full font-black tracking-tight hover:bg-slate-700 active:scale-95 transition-all shadow-lg shrink-0"
      >
        <MagnifyingGlassIcon class="size-5" /> <span>Search</span>
      </button>
    </div>
  </form>
</template>

<script setup>
import { MagnifyingGlassIcon } from '@heroicons/vue/24/solid'
</script>
