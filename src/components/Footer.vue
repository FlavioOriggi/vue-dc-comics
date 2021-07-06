<template>
  <footer>
    <div class="footer-high">
      <div class="container-up">
          <div class="footer-list">
            <div class="comics-e-shop"> 
              <div class="comics">
                <h5>dc comics</h5>
                <ul>
                  <li><a href=""></a></li>                  
                </ul>              
              </div>

              <div class="shop">
                <h5>shop</h5>
                <ul>
                  <li><a href=""></a></li>                  
                </ul>              
              </div>                    
            </div>

            <div class="dc"> 
              <h5>dc</h5>
                <ul>
                  <li><a href=""></a></li>                 
                </ul>      
            </div>
            <div class="sites">  
              <h5>sites</h5>
                <ul>
                  <li><a href=""></a></li>                    
                </ul>    
            </div>
          </div> 

          <div class="logo-sfondo">
            <img src="../assets/dc-logo-bg.png" alt="">
          </div>        
      </div> 
    </div> 
    <div class="footer-low">
      <div class="container-low">
          <div class="button-footer-low">
            <button><a href="">sign-up now!</a></button>            
          </div>            
          <div class="follow-icons">
            <h5>follow use</h5>
            <img src="../assets/footer-facebook.png" alt="">
            <img src="../assets/footer-twitter.png" alt="">
            <img src="../assets/footer-youtube.png" alt="">
            <img src="../assets/footer-pinterest.png" alt="">
            <img src="../assets/footer-periscope.png" alt="">                    
          </div>        
      </div> 
    </div>  
            
  </footer>   
</template>

<script>
export default {
  item: "Footer"
  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">


.footer-high{    
  background-image:url("../assets/footer-bg.jpg");
  height: 400px;
  padding: 50px 0;  

  .container-up{
    width: 75%; 
    margin: 0 auto;

    .footer-list{
      width: 33%;
      display: flex;

      .comics-e-shop, .dc,
      .sites{
        width: 33%;
        padding: 5px;

        h5{
          text-transform: uppercase;
          color: white;  
          font-size: 20px;
        }

        ul{
          margin-top: 10px;
          list-style: none;

          li{
            display: inline-block;
            padding:60px 0;
            margin: 0 10px;

            a{
              color: #5b5f55;
              font-size: 20px;
              font-weight: bold;
              text-decoration: none;                

              // &:hover,
              // &.active{
              //     background-color: blueviolet;
              // }
            }
          }
        }    
      }
    }
      
  } 
}

.footer-low{
  background-color: #303030;
  height: 130px;

  .container-low{
        width: 75%;
        display: flex;
        justify-content: space-between;               
        margin: 0 auto;
        padding: 50px 0;


        .follow-icons{
          display: flex;

          h5{
            color: #0282f9;
            text-transform: uppercase;
            font-size: 20px;
            margin-right: 10px;
            padding-top: 5px;
          }

          img{
            margin: 0 10px
          }
        }

        .logo-sfondo{
          img{
            width: 50%;
          }
        }


  }
}
</style>