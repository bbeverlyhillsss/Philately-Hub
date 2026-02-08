<template>
  <li>
    <a
      v-bind="$attrs"
      class="flex items-center gap-2 px-6 py-2 rounded-full bg-slate-800 text-white font-black tracking-tight transition-all duration-300 hover:scale-110 hover:bg-slate-700 hover:shadow-xl cursor-pointer active:scale-95 capitalize"
    >
      <slot></slot>
    </a>
  </li>
</template>

<script>
export default {
  inheritAttrs: false,
}
</script>
