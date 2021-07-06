<template>
  <section class="products">
    <div class="container">
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-comics-digital-comics.png" alt="">
        <h5>Digital Comics</h5>
      </div>
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-comics-merchandise.png" alt="">
        <h5></h5>
      </div>
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-comics-subscriptions.png" alt="">
        <h5></h5>
      </div>
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-comics-shop-locator.png" alt="">
        <h5></h5>
      </div>
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-dc-power-visa.svg" alt="">
        <h5></h5>
      </div>
      

      
      
       
    </div>       
  </section>
</template>

<script>
export default {
  item: "Products",
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">

.products{
  display: flex;
  
  background-color: #0282f9;
  height: 180px;
  padding: 60px 0;

  .container{

    width: 75%;
    display: flex;
    justify-content: space-around;     
    margin: 0 auto;

    .icon-contenent{
      display: flex;

      .img-products{
        width: 5%;
      }

    }

      
  }
}
</style>