
<template>
  <div class="info-cards">
    <h3 class="title">{{ cards.title }}</h3>
    <div class="cards">
      <InfoCard
        v-for="card in cards.cards"
        :key="card.title"
        :title="card.title"
        :text="card.text"
        :img="card.imagePath"
      ></InfoCard>
    </div>
  </div>
</template>

<script setup>
const { cards } = defineProps([
  'cards',
])
</script>

<style scoped>
.info-cards {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 120px;
  margin: 0 108px;
}
.title {
  margin: 0;
  font-weight: var(--font-header-info--weight);
  font-size: var(--font-header-info--size);
  line-height: var(--font-header-info--line-height);
  color: var(--font-header-info--color);
}
.cards {
  display: flex;
  gap: 200px;
}
</style>
