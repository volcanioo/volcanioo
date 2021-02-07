<template>
  <div class="grid sm:grid-rows-1 md:grid-cols-5 md:my-xl sm:my-l sm:w-full sm:mx-auto bg-white shadow-2 rounded-sm transition-all hover:transform hover:-translate-y-xs hover:shadow-6">
    <figure class="md:col-span-2 relative">
      <img 
        src="https://homeday.imgix.net/https%3A%2F%2Fd1wt9mgyrr09vn.cloudfront.net%2Fimages%2Fconnect_photos%2FL%2FC%2F1%2FX%2FLC1XS73V%2F085ada716a.jpg?ixlib=js-2.3.2&w=500&fit=crop&crop=focalpoint&s=31c4465f9552f150d8b058a1fb24543c" 
        alt="Image"
        class="block w-full h-full sm:max-h-3xl object-cover"
      />
      <a href="#" class="absolute w-full h-full block top-0 left-0"></a>
    </figure>
    <article class="md:col-span-3 p-m grid">
      <a 
        class="text-2xl font-bold text-primary-100 hover:text-primary-110"
        href="#"
        v-text="'Bruderhofstraße 40, 78224 Singen (Hohentwiel)'"
      />
      <span class="text-xl text-primary-100"> €198.435 | 2.5 Zimmer</span>
      <p class="my-m text-lg font-semibold flex flex-row items-center">
        <img src="https://my.homeday.de/img/ic_time--outline.f2faacd4.svg" alt="icon">
        <span class="ml-m">13. Februar 2021, 11:30–11:50 Uhr</span>
      </p>
      <button class="flex-1 px-l py-s w-max border-2 border-primary-110 text-primary-110 hover:bg-primary-110 hover:shadow-5 hover:text-white transition duration-300 max-h-full sm:w-full">
        <span class="text-base leading-snug font-semibold">Secondary Button</span>
      </button>
    </article>
  </div>
</template>

<script>
export default {
  name: "Card",
}
</script>