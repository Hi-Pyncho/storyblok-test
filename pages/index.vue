<template>
  <div>
    <StoryblokComponent v-if="story" :blok="story.content"></StoryblokComponent>
  </div>
</template>

<script setup>
  const story = await useStoryblok('home', {
    version: 'draft',
    resolve_relations: "featuredProjects.projects",
  },
  // {
  //   resolve_relations: "featuredProjects.projects",
  // }
  )
</script>
