<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Tiptap from './components/Tiptap.vue'

</script>

<template>
  <div>
    <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/WriteArticle">WriteArticle</RouterLink>
      </nav>
    </header>
  
    <RouterView />
  </div>
</template>

<style scoped>

nav {
  width: 100%;
  height: 70px;
  background-color: rgb(102, 255, 0);
  color: white;
  margin-right: 20px;
  position: fixed;
}

</style>
