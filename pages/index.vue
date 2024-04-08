<template>
  <div class="page-wrapper">
    <div class="main-level-wrapper">
      <div class="main-level">
        <h1 class="header-main">
          Мы делаем <br> регистрацию <br> простой и понятной
        </h1>
        <p class="text-main">Получайте SMS-сообщения онлайн на виртуальный номер для регистрации в различных социальных сетях, интернет-магазинах и онлайн-сервисах абсолютно анонимно</p>
        <Button text="Начать"></Button>
      </div>
    </div>

    <div class="info-cards-wrapper">
      <div v-for="card in cards">
        <Info :cards="card"></Info>
      </div>
    </div>
  </div>
</template>

<script setup>
const cards = [
  {
    title: 'Как это работает?',
    cards: [
      {
        imagePath: '/Users.svg',
        title: 'Регистрация',
        text: 'Регистрация на нашем сайте - мгновенный и анонимный процесс, обеспечивающий максимальный комфорт и безопасность.'
      },
      {
        imagePath: '/Id.svg',
        title: 'Получение номера',
        text: 'Получите виртуальный номер в личном кабинете, скопируйте и вставьте его в нужный сервис для получения SMS-сообщения.'
      },
      {
        imagePath: '/Chat.svg',
        title: 'Получение кода',
        text: 'После получения SMS-сообщения в вашем личном кабинете будет доступен уникальный код для регистрации.'
      },
    ]
  },
  {
    title: 'Как это работает?',
    cards: [
      {
        title: 'Регистрация',
        text: 'Регистрация на нашем сайте - мгновенный и анонимный процесс, обеспечивающий максимальный комфорт и безопасность.'
      },
      {
        title: 'Регистрация',
        text: 'Регистрация на нашем сайте - мгновенный и анонимный процесс, обеспечивающий максимальный комфорт и безопасность.'
      },
      {
        title: 'Регистрация',
        text: 'Регистрация на нашем сайте - мгновенный и анонимный процесс, обеспечивающий максимальный комфорт и безопасность.'
      },
    ]
  },
]
</script>

<style scoped>
.page-wrapper {
  height: 100%;
}

.main-level-wrapper {
  padding: 208px 0 0 251px;
  background-image: url('@/assets/gradientShape.svg');
  background-size: cover;
  background-repeat: no-repeat;
  margin-bottom: 259px;
}
.main-level {
  display: flex;
  flex-direction: column;
  gap: 62px;
  width: 45%;
}
.header-main {
  margin: 0;
  font-weight: var(--font-header-main--weight);
  font-size: var(--font-header-main--size);
  line-height: var(--font-header-main--line-height);
  letter-spacing: var(--font-header-main--letter-spacing);
}
.text-main {
  color: #1D3043;
  margin: 0;

  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: 34px;
}
</style>
