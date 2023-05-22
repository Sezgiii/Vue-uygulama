<template>
 <div>
   <Active></Active>
    <Navbar></Navbar>
  <router-view/>
 
 </div>
</template>

<script>
import Active from './components/Active.vue'
import Navbar from './components/Navbar.vue'
export default {
  components: {
    Navbar,
    Active
  },
 
}
</script>

<style>
body{
  background: #f2f2f2;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  max-width: 600px;
  margin: 0 auto;
  color: #555;
}


</style>
