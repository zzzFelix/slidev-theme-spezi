<template>
  <div class="slidev-layout cover">
    <div class="my-auto w-full">
      <slot />
    </div>
  </div>
</template>

<style>
.slidev-layout.cover {
  @apply h-full grid;
  text-align: center;

  h1 {
    @apply text-6xl leading-20;
  }

  h1+p {
    @apply text-4xl;
  }

  p+h2,
  ul+h2,
  table+h2 {
    @apply mt-10;
  }
}
</style>
