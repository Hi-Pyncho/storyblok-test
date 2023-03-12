<template>
  <div>
    <StoryblokComponent
      v-for="blokEl in blok.body"
      :key="blokEl._uid"
      :blok="blokEl"
    ></StoryblokComponent>
  </div>
</template>

<script setup>
  defineProps({
    blok: Object,
  })
</script>
