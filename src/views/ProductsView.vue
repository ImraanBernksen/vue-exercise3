<template>
  <NavBar/>
  <h1>Products</h1>
  <Products/>
  <Footer/>
</template>
<script>
import NavBar from '../components/NavBar.vue';
import Products from '../components/Products.vue';
import Footer from '../components/Footer.vue'
export default {
  components: {
    NavBar,
    Products,
    Footer
  }
}
  </script>
  <style scoped>
    
  </style>