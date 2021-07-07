<template>
  <footer>
    <div class="footer-high">
      <div class="container-up">
          <div class="footer-list">
            <div class="comics-e-shop"> 
              <div class="comics">
                <h5>dc comics</h5>
                <ul>
                  <li v-for="(item,i) in dcComics" :key="i"><a :href="item.link"> {{item.text}} </a></li>                 
                </ul>              
              </div>

              <div class="shop">
                <h5>shop</h5>
                <ul>
                  <li v-for="(item,i) in shop" :key="i"><a :href="item.link"> {{item.text}} </a></li>                  
                </ul>              
              </div>                    
            </div>

            <div class="dc"> 
              <h5>dc</h5>
                <ul>
                  <li v-for="(item,i) in dc" :key="i"><a :href="item.link"> {{item.text}} </a></li>                 
                </ul>      
            </div>
            <div class="sites">  
              <h5>sites</h5>
                <ul>
                  <li v-for="(item,i) in sites" :key="i"><a :href="item.link"> {{item.text}} </a></li>                    
                </ul>    
            </div>
          </div> 

          <div class="logo-sfondo">            
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
  name: 'Footer',
  data(){
    return{
      dcComics : [
        {
          text : 'Characters',
          link : '#'
        },
        {
          text : 'Comics',
          link : '#'
        },
        {
          text : 'Movies',
          link : '#'
        },
        {
          text : 'TV',
          link : '#'
        },
        {
          text : 'Games',
          link : '#'
        },
        {
          text : 'Videos',
          link : '#'
        },
        {
          text : 'News',
          link : '#'
        }
      ],
      shop : [
        {
          text : 'Shop DC',
          link : '#'
        },
        {
          text : 'Shop DC Collectibles',
          link : '#'
        }
      ],
      dc : [
        {
          text : 'Terms Of Use',
          link : '#'
        },
        {
          text : 'Privacy policy (New)',
          link : '#'
        },
        {
          text : 'Ad Choices',
          link : '#'
        },
        {
          text : 'Advertising',
          link : '#'
        },
        {
          text : 'Jobs',
          link : '#'
        },
        {
          text : 'Subscriptions',
          link : '#'
        },
        {
          text : 'Talent Workshops',
          link : '#'
        },
        {
          text : 'CPSC Certificates',
          link : '#'
        },
        {
          text : 'Rating',
          link : '#'
        },
        {
          text : 'Shop Help',
          link : '#'
        },
        {
          text : 'Contact Us',
          link : '#'
        }
      ],
      sites : [
        {
          text : 'DC',
          link : '#'
        },
        {
          text : 'MAD Magazine',
          link : '#'
        },
        {
          text : 'DC Kids',
          link : '#'
        },
        {
          text : 'DC Universe',
          link : '#'
        },
        {
          text : 'DC Power Visa',
          link : '#'
        }
      ]     
    }
  },
  methods : {
    getImgUrl(pic) {
      return require('../assets/footer-' + pic + '.png')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">


.footer-high{    
  background-image:url("../assets/footer-bg.jpg");
  background-size: cover;    

  .container-up{
    width: 75%; 
    margin: 0 auto;
    display: flex;

    .footer-list{
      width: 33%;
      display: flex;
      padding: 50px 0; 

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

    .logo-sfondo{  
      background-image: url('../assets/dc-logo-bg.png');
      width: 50%; 
      
      background-size: cover;
      background-position: center;
    }        
  } 
}

.footer-low{
  background-color: #303030;  
  padding: 50px 0;

  .container-low{
    width: 75%;
    display: flex;
    justify-content: space-between; 
    align-items: center;            
    margin: 0 auto;        

      button{
        padding: 10px 15px; 
        border: 2px solid #0282f9;
        text-transform: uppercase;
        color: white;
        font-size: 18px;
        background-color: #303030;

        a{
          color: white;
          text-decoration: none;
        }          
      }


      .follow-icons{
        display: flex;

        h5{
          color: #0282f9;
          text-transform: uppercase;
          font-size: 20px;
          margin-right: 10px;
          padding-top: 7px;           
        }

        img{
          margin: 0 10px
        }
      }
  }
}
</style>