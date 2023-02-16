<template>
  <div class="slidev-layout fact">
    <div class="my-auto">
      <slot />
    </div>
  </div>
</template>

<style>
.slidev-layout.fact {
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
  