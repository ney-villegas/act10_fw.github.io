
<template>
  <div @click="openCategoryList" class="category-container" >
  <img :src="category.strCategoryThumb" alt="">
  <h3>{{category.strCategory}}</h3>
  <p>{{category.strCategoryDescription}}</p>
  </div>
  
  </template>
  
  <script>
  export default{
    props:["category"],
    methods:{
      openCategoryList(){
        console.log(this.category)
        this.$router.push("/category/" + this.category.strCategory)
        console.log(this.category.strCategory)
      }
      
    }
  }
  </script>