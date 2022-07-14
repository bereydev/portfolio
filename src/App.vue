<script setup lang="ts">
// https://github.com/vueuse/head
// you can use this to manipulate the document head in any components,
// they will be rendered correctly in the html results with vite-ssg
useHead({
  title: 'Bereyziat Development',
  meta: [
    { name: 'description', content: 'Welcome to Bereyziat Development. A dynamic team of developers seeking for the perfect code to make your projects come to life.' },
  ],
})
</script>

<template>
  <router-view />
</template>
