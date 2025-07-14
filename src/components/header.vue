<template>
  <header class="header">
    <h1 class="logo">Мой Сайт</h1>
    <nav class="nav">
      <button @click="onHomeClick">Главная</button>
      <button @click="onAboutClick">О сайте</button>
    </nav>
  </header>
</template>

<script setup>
const onHomeClick = () => {
  console.log('Переход на главную');
}

const onAboutClick = () => {
  console.log('Переход на страницу "О сайте"');
}
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  background-color: #2c3e50;
  color: white;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav button {
  margin-left: 1rem;
  padding: 0.5rem 1rem;
  background: #3498db;
  border: none;
  border-radius: 4px;
  color: white;
  cursor: pointer;
}

.nav button:hover {
  background: #2980b9;
}
</style>