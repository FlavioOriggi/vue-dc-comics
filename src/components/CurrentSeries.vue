<template>
    <section class="CurrentSeries">
        <div class="container">
            <div class="btn-series">
                <button><a href="">current series</a></button>
            </div>
            <div class="icon">  
                <!-- <img :src="currentseriesitem.thumb" :alt="currentseriesitem.series">
                <h5 class="">{{currentseriesitem.series}}</h5>        -->
                
            </div> 
            <div class="load-more">
                <button><a href="">load more</a></button>
            </div> 
        </div>    
    </section>    
</template>

<script>
export default {
  name: "CurrentSeries", 
//   props: ["currentseriesitem"]
       
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.CurrentSeries{
    background-color: #1c1c1c;

    .container{
        width: 75%;                   
        margin: 0 auto;

        .btn-series{
            button{
                padding: 10px 15px;         
                text-transform: uppercase;
                font-weight: bold;
                color: white;
                font-size: 18px;
                background-color: #0282f9;
                border: none;  
                position: relative;
                bottom: 20px;                     

                a{
                color: white;
                text-decoration: none;
                } 
            }
        }

        .icon{
            width: calc((100% - (10px * 6))/6);
            margin: 40px 0;

            img{
                margin-bottom: 10px;
            }
        }
    

        .load-more{
            display: flex;
            justify-content: center;

            button{
                padding: 10px 60px;         
                text-transform: uppercase;            
                color: white;
                font-size: 16px;
                background-color: #0282f9;
                border: none;
                margin-bottom: 15px;
            }
            a{
                color: white;
                text-decoration: none;            
            }
        }   
    }   
}

</style>