<template>
    <div class="category-container">
        <img @click="openMealList" :src="meal.strMealThumb" alt="">
        <h3>{{ meal.strMeal }}</h3>
        <p>Categoria: {{ meal.strCategory }} | Origen:{{ meal.strArea }} </p>
    </div>
</template>


<script>
export default{
    props:["meal"],
    methods:{
      openMealList(){
        //console.log(this.category)
        this.$router.push("/meal/" + this.meal.idMeal)
        //console.log(this.meal.idMeal)
      }
      
    },
}

</script>