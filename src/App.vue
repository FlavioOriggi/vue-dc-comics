<template>
  <div id="app">    
    <Header/> 
    <main>
      <Jumbotron/>
      <CurrentSeries/>
      <Products/>
    </main>     
    <Footer/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import CurrentSeries from "./components/MainItem.vue";
import Products from "./components/Products.vue";
import Footer from "./components/Footer.vue";


export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    CurrentSeries,    
    Products, 
    Footer
  }
};
</script>


<style lang="scss">

@import 'style/commons.scss';



</style>
