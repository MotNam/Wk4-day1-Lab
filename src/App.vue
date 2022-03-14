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
<a href="/views/AboutView.vue"> About Page</a><br>

<a href="/views/HomeView.vue"> Home Page</a>
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