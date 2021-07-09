<template>
    <section class="CurrentSeries">
        <div class="container">
            <div class="btn-series">
                <button><a href="">current series</a></button>
            </div>
            <div class="icon">  
                <ImgCard v-for="(card,i) in cards" :key="i" :cardData="card"/>                
            </div> 
            <div class="load-more">
                <button><a href="">load more</a></button>
            </div> 
        </div>    
    </section>    
</template>

<script>
import ImgCard from '@/components/CurrentIcon.vue';
import currentseriesitem from '@/data/currentseriesitem.js';

export default {
    name: "MainItem", 
    components: {      
        ImgCard
    },    
    data(){
        return{        
            cards : currentseriesitem  
        }  
    }  
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
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
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

                &:hover,
                &.active{
                    cursor: pointer;
                    transform: scale(1.02); 
                    border: 1px solid rgb(159, 196, 255);
              }
            }
            a{
                color: white;
                text-decoration: none;            
            }
        }   
    }   
}

</style>