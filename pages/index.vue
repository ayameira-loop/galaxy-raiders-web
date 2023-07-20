<template>
  <div>
    <ul class="navigation-menu">
      <li><NuxtLink to="/game">Start Game</NuxtLink></li>
      <li><NuxtLink to="/leaderboard">Leaderboard</NuxtLink></li>
      <li><NuxtLink to="/exit">Exit Game</NuxtLink></li>
    </ul>
  </div>
</template>

<script setup>
</script>

<style scoped>
.navigation-menu {
  list-style: none;
  display: flex;
  justify-content: space-evenly;
  padding: 0;
  margin: 20px 0;
  background-color: #f5f5f5;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.navigation-menu li {
  padding: 10px 20px;
}

.navigation-menu li:hover {
  background-color: #007bff;
  color: #fff;
  cursor: pointer;
  transition: background-color 0.3s;
}

.navigation-menu li a {
  color: #333;
  text-decoration: none;
  font-size: 18px;
  font-weight: bold;
}

.navigation-menu li a:hover {
  color: #fff;
  text-decoration: none;
}
</style>
