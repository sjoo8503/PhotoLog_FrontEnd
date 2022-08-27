<template>
  <nav class="navbar">
    <div class="navbar__logo">
      <a href="/">PhotoLog</a>
    </div>
    <div class="navbar__menu">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/create">Create</RouterLink>
    </div>
  </nav>
  <RouterView></RouterView>
</template>

<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2.5rem 8rem;
  letter-spacing: 0.1rem;
  height: 30%;
  background-color: #255fb7;
  color: #fff
}

.navbar__logo {
  font-size: 3rem;
  font-weight: 700;
  font-style: italic;
}

.navbar__logo a {
  text-decoration: none;
  color: #fff;
}

.navbar__menu * {
  font-size: 2rem;
  margin-left: 3rem;
  text-decoration: none;
  color: #fff;
}
</style>