<template>
  <div class="navbar">
    <NavBarLogo></NavBarLogo>
    <nav>
      <ul>
        <li class="navbar-element">Получить SMS</li>
        <li class="navbar-element">Заработать</li>
        <li class="navbar-element">Документация</li>
        <li class="navbar-element">Блог</li>
      </ul>
    </nav>
    <div class="buttons"></div>
  </div>
</template>

<style scoped>
.navbar {
  position: absolute;
  display: flex;
  justify-content: space-between;
  align-items: center;
  top: 0;
  width: 100%;
  padding: 42px 300px 0 84px;
}

ul {
  display: flex;
  gap: 50px;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.navbar-element {
  cursor: pointer;
  color: #fff;
  font-size: 18px;
  font-weight: 700;
  line-height: 92px;
}
</style>
