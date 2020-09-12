<template>
  <div class="the-main-layout">
    <main class="the-main-layout__content">
      <slot />
    </main>
  </div>
</template>

<script>
export default {}
</script>

<style lang="stylus">
html
  height 100%

body, .the-main-layout
  min-height 100vh

.the-main-layout
  display flex
  direction column

  &__content
    flex-grow 1
</style>
