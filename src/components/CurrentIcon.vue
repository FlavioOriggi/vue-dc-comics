<template>
  <div class="card">
    <img :src="cardData.thumb" :alt="cardData.series">
    <p> {{cardData.series}} </p>
  </div>
</template>


<script>
export default {
  name : 'ImgCard',
  props: {cardData: Object}
}
</script>


<style lang="scss" scoped>
  .card{
    width: calc((100% - (10px * 6))/6);
    margin: 40px 0;
    padding: 0 5px;

    img{
      margin-bottom: 10px;
        &:hover {
            cursor: pointer;
            transform: scale(1.02);            
        }
    }

    p{
        color: white;

        &:hover {
            cursor: pointer;
            text-decoration: underline;
        }
    }
  }
</style>