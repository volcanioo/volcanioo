<template>
  <div id="app" class="font-sans">
    <div class="mx-auto md:w-8/12 sm:w-full md:mt-xl text-primary">
      <Typography />
      <Buttons />
      <Card />
    </div>
  </div>
</template>

<script>
import Typography from '@/components/Typography.vue';
import Buttons from '@/components/Buttons.vue';
import Card from '@/components/Card.vue';

export default {
  name: 'App',
  components: {
    Typography,
    Buttons,
    Card,
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital,wght@0,200;0,300;0,400;0,600;0,700;0,900;1,200;1,300;1,400;1,600;1,700;1,900&display=swap');
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";

body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: antialiased;
}

/*! 
 * Typography
 *
 * https://tailwindcss.com/docs/line-height
 * https://tailwindcss.com/docs/font-weight
 * https://tailwindcss.com/docs/font-size
 */
h1 {
  @apply text-2xl leading-snug font-black;
}
h2 {
  @apply text-xl leading-snug font-semibold;
}
h3 {
  @apply text-lg leading-relaxed font-semibold;
}
h4 {
  @apply text-base leading-normal font-semibold;
}
h5 {
  @apply text-base leading-normal font-semibold;
}
p {
  @apply text-base leading-normal font-normal;
}
</style>
