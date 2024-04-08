<template>
  <div class="card">
    <img class="card-img" :src="img">
    <div class="card-title">{{ title }}</div>
    <div class="card-text">{{ text }}</div>
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
  align-items: center;
  gap: 30px;
}

.card-img {
  width: 146px;
}

.card-title {
  margin: 0;
  color: #3D3ABA;

  text-align: center;
  font-size: 40px;
  font-style: normal;
  font-weight: 700;
  line-height: 107%;
}

.card-text {
  text-align: center;
  font-size: 25px;
  font-style: normal;
  font-weight: 500;
  line-height: 126.5%;
}
</style>
