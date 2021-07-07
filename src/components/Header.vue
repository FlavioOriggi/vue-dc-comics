<template>
    <header>
        <div class="header-up">
            <div class="container">
                <div class="logo-container">
                    <img src="../assets/dc-logo.png" alt="">
                </div>            
                <div class="nav-bar">
                    <nav>
                        <ul>
                            <li v-for="(link, index) in links" :key="index" :class="{ active: link.current }"><a href="link.url" >{{link.text}}</a></li>
                            
                        </ul>
                    </nav>
                </div>
            </div>
        </div>        
    </header>  
</template>

<script>
export default {
  name: "Header",
  data() {
      return{
          links: [
              {
                  text: 'Characters',
                  url: '#',
                  current: false
              },
              {
                  text: 'Comics',
                  url: '#',
                  current: false
              },
              {
                  text: 'Movie',
                  url: '#',
                  current: false
              },
              {
                  text: 'TV',
                  url: '#',
                  current: true
              },
              {
                  text: 'Games',
                  url: '#',
                  current: false
              },
              {
                  text: 'Videos',
                  url: '#',
                  current: false
              },
              {
                  text: 'Fans',
                  url: '#',
                  current: false
              },
              {
                  text: 'News',
                  url: '#',
                  current: false
              },
              {
                  text: 'Shop',
                  url: '#',
                  current: false
              }
        
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{     
    .header-up{
        height: 130px;        

        .container{
        width: 75%;
        display: flex;
        justify-content: space-between;        
        margin: 0 auto;

            .logo-container{
                padding:20px 0;
                img{
                    width: 80%;
                }
            }

            ul{
                list-style: none;

                li{
                    display: inline-block;
                    padding:50px 0;
                    margin: 0 10px;


                    a{
                        color: #5b5f55;
                        font-size: 20px;
                        font-weight: bold;
                        text-decoration: none;                

                            &:hover {
                                border-bottom: 3px solid #0282f9;
                            }
                    }        
                }
            }
        }           
    }   
}
</style>