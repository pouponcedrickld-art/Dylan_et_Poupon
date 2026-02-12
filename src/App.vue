<script setup>
import { RouterLink, RouterView } from 'vue-router';

const routes = [
  {path:'/blog' , title: "Blog"},
  {path:'/' , title: "home"},
]
</script>

<template>
<nav>

  <RouterLink to="/">home</RouterLink>
  <RouterLink to="/blog"> Blog</RouterLink>
</nav>
<RouterView ></RouterView>
</template>

<style scoped>
nav {
  display: flex;
  gap: 15px;
  padding: 20px;
  background: #f4f4f4;
  display: flex;
  justify-content: center;
}

a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
}

a.router-link-active {
  color: #42a1b8;
  /* border-bottom: 2px solid #428db88c; */
}
</style>

