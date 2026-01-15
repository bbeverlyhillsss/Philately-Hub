<template>
  <div class="min-h-screen bg-linear-to-b from-[#94B0DA] to-[#CBD5E1] text-slate-900 font-sans">
    <header class=" p-4 border-b border-white/0">
      <nav class="max-w-7xl mx-auto">
        <ul class="flex items-center justify-between gap-4">
          <li class="shrink-0">
            <a href="/" class="block group">
              <img
                src="./assets/stamp-svgrepo-com.svg"
                alt="Logo"
                class="size-10 md:size-12 group-hover:scale-110 group-hover:rotate-3 transition-all duration-300"
              />
            </a>
          </li>
          <div class="flex flex-wrap gap-10 items-center">
            <li
              class="flex items-center gap-2 px-6 py-2 rounded-full bg-slate-800 text-white font-black tracking-tight transition-all duration-300 hover:scale-110 hover:bg-slate-700 hover:shadow-xl cursor-pointer active:scale-95"
            >
              <HomeIcon class="size-5"/><span> Home Page</span>
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
          </div>
        </ul>
      </nav>
    </header>

    <main class="max-w-7xl mx-auto px-6 py-16 md:py-24">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
        <div class="space-y-8">
          <h1
            class="text-4xl md:text-5xl xl:text-6xl font-black text-slate-800 tracking-tighter leading-tight"
          >
            Discover Rare Stamps from Around the World
          </h1>

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
                class=" flex items-center gap-2 bg-slate-800 text-white px-8 py-3 rounded-full font-black tracking-tight hover:bg-slate-700 active:scale-95 transition-all shadow-lg shrink-0"
              >
                <MagnifyingGlassIcon class="size-5"/> <span>Search</span>
              </button>
            </div>
          </form>
        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
import { HomeIcon, RectangleStackIcon, UserIcon, MagnifyingGlassIcon } from '@heroicons/vue/24/solid'
</script>

<style>
body {
  margin: 0px;
  padding: 0px;
}
</style>
