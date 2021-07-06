<template>
  <section class="products">
    <div class="container">
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-comics-digital-comics.png" alt="">
        <p class="text-icon-products">digital Comics</p>
      </div>
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-comics-merchandise.png" alt="">
        <p class="text-icon-products">dc merchandise</p>
      </div>
      <div class="icon-contenent">
        <img class="img-products" src="../assets/buy-comics-subscriptions.png" alt="">
        <p class="text-icon-products">subscriptions</p>
      </div>
      <div class="icon-contenent">
        <img class="img-locator-products" src="../assets/buy-comics-shop-locator.png" alt="">
        <p class="text-icon-products">comics shop locator</p>
      </div>
      <div class="icon-contenent">
        <img class="img-visa-products" src="../assets/buy-dc-power-visa.svg" alt="">
        <p class="text-icon-products">dc power visa</p>
      </div>
    </div>       
  </section>   
</template>

<script>
export default {
  item: "Products",
  data() {
      return {          
          listProducts: [                
          ]
      }
  }
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
      width: 20%;

      .img-products{
        width: 20%;
        margin-right: 5px;
      }

      .text-icon-products{
        color: white;
        text-transform:uppercase;
        font-size: 16px;
        padding: 20px 0;       
      }

      .img-locator-products{
        width: 15%;
        margin-right: 5px;
      }

      .img-visa-products{   
        width: 70px;
        margin-right: 5px;
      }
    }      
  }
}
</style>