<template>

  <section>

    <div class="blue-bar-container">
  
      <div class="card">
  
        <div>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        </div>
  
        <div>
          <span>digital comics</span>
        </div>
  
      </div>
      <div class="card">
  
        <div>
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
        </div>
  
        <div>
          <span>dc merchandise</span>
        </div>
  
      </div>
      <div class="card">
  
        <div>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        </div>
  
        <div>
          <span>subscription</span>
        </div>
  
      </div>
      <div class="card">
  
        <div>
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        </div>
  
        <div>
          <span>comic shop locator</span>
        </div>
  
      </div>
      <div class="card">
  
        <div>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        </div>
  
        <div>
          <span>dc power visa</span>
        </div>
  
      </div>
  
    </div>

  </section>

  
</template>

<script>
export default {
  name: "BlueBar"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/variable.scss";

section{
  
  width: 100%;
  background-color: $primary-color;
  height: 150px;

   display: flex;
    justify-content: center;
    align-items: center;


  .blue-bar-container{

    width: 70%;
    margin: 0 auto;

    display: flex;
    justify-content: space-around;
    align-items: center;

    color: white;

      .card{
        display: flex;
        justify-content: center;
        align-items: center;

          img{
            width: 40px;
            margin-right: 10px;
          }

          span{
            text-transform: uppercase;
            font-size: 14px;

          }

      }

  }

}



</style>