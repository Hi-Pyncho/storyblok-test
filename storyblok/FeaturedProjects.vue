<template>
  <div class="container" v-editable="blok">
    <h2 style="margin-left: 10px">{{ blok.title }}</h2>
    <div class="featured-projects">
      <div class="project" v-for="project in blok.projects" :key="project._uid">
        <NuxtLink
          :to="{ name: 'projects-slug', params: { slug: project.slug } }"
        >
          <h3> 123 </h3>
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  blok: Object,
});
</script>
