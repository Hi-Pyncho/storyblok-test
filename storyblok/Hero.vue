<template>
  <div class="hero">
    <div class="container">
      <div class="col">
        <img :src="blok.image.filename" :alt="blok.image.alt">
      </div>
      <div class="col">
        <h2>
          {{ blok.title }}
        </h2>
        <p>
          <b>
            {{ blok.subtitle }}
          </b>
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
  defineProps({
    blok: Object,
  })
</script>
