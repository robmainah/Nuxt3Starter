<script setup lang="ts">
const route = useRoute();
useHead({
  title: route.params.name.toString().toUpperCase(),
});

definePageMeta({
  layout: 'custom'
})
</script>

<template>
  <div>
    <CarDetailHero />
    <CarDetailAttributes />
    <CarDetailDescription />
    <CarDetailContact />
  </div>
</template>