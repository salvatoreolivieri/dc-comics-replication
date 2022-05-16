<template>

  <main>

    <section class="hero-section">
      <button>current series</button>
    </section>

    <section>

      <div class="card-section">

        <div class="card-element">
          <img src="../assets/img/1.jpg" alt=""><br>
          <span>ciao</span>
        </div>
        <div class="card-element">
          <img src="../assets/img/1.jpg" alt=""><br>
          <span>ciao</span>
        </div>
        <div class="card-element">
          <img src="../assets/img/1.jpg" alt=""><br>
          <span>ciao</span>
        </div>
        <div class="card-element">
          <img src="../assets/img/1.jpg" alt=""><br>
          <span>ciao</span>
        </div>
        <div class="card-element">
          <img src="../assets/img/1.jpg" alt=""><br>
          <span>ciao</span>
        </div>
        <div class="card-element">
          <img src="../assets/img/1.jpg" alt=""><br>
          <span>ciao</span>
        </div>
        <div class="card-element">
          <img src="../assets/img/1.jpg" alt=""><br>
          <span>ciao</span>
        </div>
      </div>

      <div class="load-more-button-container">
        <button class="load-more-button">load more</button>
      </div>

    </section>

  </main>
  
</template>

<script>
export default {
  name: "MainComponent"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/variable";

  main{
    // width: 80%;
    margin: 0 auto;
    background-color: #1C1C1C;
    color: white;

    .hero-section{
      background-image: url("../assets/img/jumbotron.jpg");
      background-size: cover;
      height: 400px;
      width: 100%;
      position: relative;

      button{
        position: absolute;
        bottom: -24px;
        left: 217px;

        background-color: $primary-color;
        border: none;
        padding: 15px;
        text-transform: uppercase;
        color: white;
        font-weight: bold;
        font-size: 16px;

      }

    }

    .card-section{
      width: 70%;
      margin: 0 auto;
      border: 1px solid white;
      padding: 45px 10px;
      display: flex;
      flex-wrap: wrap;


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


    }

    .load-more-button-container{
      display: flex;
      justify-content: center;
      align-items: center;
      height: 70px;


      .load-more-button{
        background-color: $primary-color;
        border: none;
        padding: 10px 45px;
        color: white;
        text-transform: uppercase;
        font-size: 11px;
        font-weight: bold;

        cursor: pointer;
      }

    }



  }

</style>