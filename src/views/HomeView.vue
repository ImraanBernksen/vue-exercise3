<template>
  <NavBar/>
  <h1>Home</h1>
  <Footer/>
</template>
<script>
import NavBar from '../components/NavBar.vue';
import Footer from '../components/Footer.vue'
export default {
  name: 'HomeView',
  components: {
    NavBar,
    Footer
  }
}
</script>
<style scoped>
  
</style>