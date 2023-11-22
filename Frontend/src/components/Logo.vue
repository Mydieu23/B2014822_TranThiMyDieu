<script setup>
const { size } = defineProps({
  size: {
    required: false,
    type: Number,
    default: 35
  }
})
</script>

<template>
  <span class="logo" :style="{ fontSize: `${size}px` }">
    <router-link to="/" class="logo-content">Love Flower</router-link>
  </span>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap');

.logo {
  font-family: 'Dancing Script', cursive;
  font-weight: 700;

  &-content,
  &-content:hover {
    text-decoration: none;
    color: #bd2026;
    text-shadow: 0 1px #000;
  }
}
</style>
