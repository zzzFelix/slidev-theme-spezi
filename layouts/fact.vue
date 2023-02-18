<template>
  <div class="slidev-layout fact">
    <div>
      <slot />
    </div>
  </div>
</template>

<style>
.slidev-layout.fact {
  @apply h-full grid;
  text-align: center;
  align-items: center;

  h1 {
    @apply text-5xl leading-20;
  }

  h2 {
    @apply mb-5;
  }
}
</style>
  