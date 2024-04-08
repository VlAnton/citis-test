<template>
  <div class="card">
    <img class="card-img" :src="img">
  </div>
</template>

<script setup>
const { title, text, img } = defineProps([
  'title',
  'text',
  'img'
])
</script>

<style>
.card {
  display: flex;
  flex-direction: column;
  gap: 30px;
}
</style>
