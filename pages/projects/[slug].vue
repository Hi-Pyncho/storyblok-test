<template>
  <div>
    <StoryblokComponent v-if="story" :blok="story.content"></StoryblokComponent>
  </div>
</template>

<script setup>
  const route = useRoute()
  const story = await useStoryblok(`projects/${route.params.slug}`, {
  version: 'draft'
})
</script>
