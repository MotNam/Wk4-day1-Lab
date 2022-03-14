<template>
  <div>
    <!-- iteration 1 -->
    <p>New Component</p>
    <NewVueComp />

<!-- 　　iteration 2  -->
<span>Message:{{message}} </span>
    <!-- iteration 3 -->
<button @click = "printFunction">Click Here</button> 

<!-- iteration 4 -->
<div>
  <router-link to="home">Home</router-link>
  <router-link to="about/1/2/3">About</router-link>
  <router-view/>



<!-- <a :href="link"> About Page</a><br>
<a :href="link"> Home Page</a> -->
</div>
  </div>

</template>

<script>
import NewVueComp from './components/NewVueComp.vue'

export default {
  name: 'App',
  components: {
    NewVueComp,
  },
   data() {
    return {
      message:'Text Interpolation',
    
  }
  },
   methods: {
      printFunction(){
        console.log("Hello World");
      },
    
}
}

</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>