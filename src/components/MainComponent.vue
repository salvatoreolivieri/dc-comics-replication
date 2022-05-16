<template>

  <main>

    <section class="hero-section">
      <button>current series</button>
    </section>

    <section>

      <div class="card-section">

        <ComicsCard 
        v-for="(cardItem,index) in cardData" :key="`card-${index}`"
        :card = "cardItem"
        
        />

      </div>

      <div class="load-more-button-container">
        <button class="load-more-button">load more</button>
      </div>

    </section>

  </main>
  
</template>

<script>
import ComicsCard from './ComicsCard.vue'

// import ComicsCard from "./ComicsCard.vue";
export default {
    name: "MainComponent",
    components: { ComicsCard },

    data(){
      return{
        cardData: [
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
            price: "$19.99",
            series: "Action Comics",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
            price: "$3.99",
            series: "American Vampire 1976",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
            price: "$16.99",
            series: "Aquaman",
            type: "graphic novel"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
            price: "$2.99",
            series: "Batgirl",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
            price: "$3.99",
            series: "Batman",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
            price: "$2.99",
            series: "Batman Beyond",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
            price: "$3.99",
            series: "Batman/Superman",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
            price: "$4.99",
            series: "Batman/Superman Annual",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
            price: "$5.99",
            series: "Batman: The Joker War Zone",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
            price: "$6.99",
            series: "Batman: Three Jokers",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
            price: "$4.99",
            series: "Batman: White Knight Presents: Harley Quinn",
            type: "comic book"
          },
          {
            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
            price: "$16.99",
            series: "Catwoman",
            type: "graphic novel"
          }
        ]
      }
    }
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
      padding: 45px 10px;
      display: flex;
      flex-wrap: wrap;


      // .card-element{

      //   width: calc((100% / 6) - 20px);
      //   margin: 0px 10px;
      //   margin-bottom: 40px;

      //   img{
      //     margin-bottom: 10px;
      //     width: 100%;

      //   }
        
      //   span{
      //     text-transform: uppercase;
      //   }

      // }


    }

    .load-more-button-container{
      display: flex;
      justify-content: center;
      align-items: center;
      height: 70px;
      margin-top: -50px;


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