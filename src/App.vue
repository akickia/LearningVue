<script setup>
import { RouterLink, RouterView } from 'vue-router'
import FooterCard from '@/components/FooterCard.vue'

</script>

<template>
  <div id="layout">
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />
    <div class="wrapper">
      <nav>
        <RouterLink :to="{ name: 'event-list'}">Events</RouterLink> |
        <RouterLink :to="{ name: 'about'}">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
  <FooterCard />
</div>
</template>

<style >
body {
  margin: 0
}
#layout {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding-bottom: 6rem;
}
nav {
  padding: 30px;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
}
nav a.router-link-exact-active {
  color: #42b983;
}

h2 {
  font-size: 20px;
}
</style>
