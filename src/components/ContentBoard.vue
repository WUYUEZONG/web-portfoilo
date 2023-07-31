<template>
  <div class="align-center">
    <div class="limit-width">
        <slot />
    </div>
  </div>
</template>

<style scoped>
.align-center {
  display: flex;
  justify-content: center;
}

.limit-width {
  max-width: 1100px;
  width: calc(100vw - 10%);
}
</style>