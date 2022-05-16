<template>

    <div class="card-element">
        <img :src="card.thumb" alt=""><br>
        <span>{{card.series}}</span>
    </div>

</template>

<script>
export default {
  name:"ComicsCard",
  props:{
        card: Array
    }
}
</script>

<style lang="scss" scoped>

.card-element{

        width: calc((100% / 6) - 20px);
        margin: 0px 10px;
        margin-bottom: 40px;

        img{
          margin-bottom: 10px;
          width: 100%;

        }
        
        span{
          text-transform: uppercase;
        }

      }

</style>