<template>
  <div class="md:shadow-7 rounded-md from-purple-100 p-m md:mb-l">
    <h1 class="mb-m border-b border-blue-200 pb-xs">Buttons</h1>

    <div class="grid grid-cols-2 gap-l">
      <button class="flex-1 px-l py-s bg-primary-110 shadow-3 hover:shadow-5 transition duration-300">
        <span class="text-base leading-snug text-white font-semibold">Primary Button</span>
      </button>

      <button class="flex-1 px-l py-s border-2 border-primary-110 text-primary-110 hover:bg-primary-110 hover:shadow-5 hover:text-white transition duration-300">
        <span class="text-base leading-snug font-semibold">Secondary Button</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Buttons",
}
</script>