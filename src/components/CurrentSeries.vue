<template>
    <section class="CurrentSeries">
        <div class="btn-series">
            <button><a href="">current series</a></button>
        </div>
        <div class="icon-series">            
            <img src="" alt="">
            <div> </div>
        </div> 
        <div class="load-more">
            <button><a href="">load more</a></button>
        </div>     
    </section>    
</template>

<script>
export default {
  name: "CurrentSeries", 
  props: {cardData: Object}  
       
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.CurrentSeries{
    background-color: #1c1c1c;
    

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
            left: 50px;

            a{
            color: white;
            text-decoration: none;
            } 
        }
    }

    .icon-series{
        width: calc((100% - (10px * 6))/6);
        margin: 50px 0;
        img{
            margin-bottom: 20px;
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

        }

        a{
            color: white;
            text-decoration: none;
            
        }
    }

    
}

</style>