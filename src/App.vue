<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Category from './components/Category.vue'
import Meals from './components/Meals.vue'
import swal from 'sweetalert'
import axios from 'axios'
</script>

<template>
  <div>
      <img src="../public/logo.jpeg" class="logo vue" alt="Vue logo" />
  </div>
  <HelloWorld msg="FastFood" />

  <nav id="nav">
    <router-link to="/">/ Inicio /</router-link>
    <router-link to="/ categoryDetails"> CategoryDetails /</router-link>
    <router-link to="/mealsDetails"> MealsDetails /</router-link>
  </nav>
  <router-view></router-view>

  
</template>

<script>
export default{
  name:'App',
  
}
</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #a8adffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #345345aa);
}
.category-container{
  border-radius: 10px;
  color: black;
  margin: 5% 20%;
  background-color: gray;


}
</style>
