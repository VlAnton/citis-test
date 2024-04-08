<template>
  <div class="button" :class="className ? className : ''">
    {{ text }}
  </div>
</template>

<script setup>
const { text, className } = defineProps([
  'text',
  'className'
])
</script>

<style scoped>
.button {
  padding: 14px 40px;
  background-color: var(--button-background-color--primary);
  box-shadow: 0px 26px 7px 0px rgba(26, 56, 116, 0.00),
              0px 17px 7px 0px rgba(26, 56, 116, 0.01),
              0px 9px 6px 0px rgba(26, 56, 116, 0.05),
              0px 4px 4px 0px rgba(26, 56, 116, 0.09),
              0px 1px 2px 0px rgba(26, 56, 116, 0.10);
  border-radius: 14px;
  width: fit-content;

  font-size: 20px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  letter-spacing: -0.4px;

  color: #fff;

  cursor: pointer;
}

.button--rounded {
  box-shadow: none;
  background-color: var(--button-background-color--secondary);
  border-radius: 64px;

  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;

  padding: 16px 31.5px;
}
</style>
