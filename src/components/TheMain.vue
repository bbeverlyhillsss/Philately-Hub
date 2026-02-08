<template>

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


</template>



<script setup>
import { MagnifyingGlassIcon } from '@heroicons/vue/24/solid'



</script>