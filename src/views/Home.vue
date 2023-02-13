<template>
  <Splash />
</template>

<script lang="ts" setup>
  import Splash from '@/components/Splash.vue'
</script>

<style>
html {
  overflow: hidden !important;
  scrollbar-width: none;
  -ms-overflow-style: none;
}

html::-webkit-scrollbar {
  width: 0;
  height: 0;
}
</style>