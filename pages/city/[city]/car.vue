<script setup lang="ts">
const route = useRoute();

useHead({
  title: `${route.params.make ? route.params.make.toString() : 'Cars'} in ${route.params.city.toString().toUpperCase()}`,
});

definePageMeta({
  layout: 'custom',
})
</script>

<template>
  <div class="mt-32 flex">
    <CarSidebar />
    <NuxtPage />
  </div>
</template>