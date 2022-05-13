<template>

  <footer>

    <div class="top-footer-background">

        <div class="top-footer-content">

          <div class="top-footer-content-links">

            <div class="column-footer-links">

              <h3>dc comics</h3>

              <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
              </ul>


              <h3>shop</h3>

              <ul>
                <li><a href="#">Shop DC</a></li>
                <li><a href="#">Shop DC Collectibles</a></li>
              </ul>

            </div>

            <div class="column-footer-links">

              <h3>dc</h3>

              <ul>
                <li><a href="#">Term Of Use</a></li>
                <li><a href="#">Privacy Policy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Rating</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
              </ul>

              
            </div>

            <div class="column-footer-links">

              <h3>sites</h3>

              <ul>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
              </ul>

            </div>

          </div>

          <div class="top-footer-content-dc-background">
            <!-- qui è stato messo il background con il logo DC -->
          </div>

        </div>

    </div>

    <div class="bottom-footer">

        <div class="bottom-footer-content">

          <div>
            <button href="#">sign-up now</button>
          </div>


          <div class="social-container">

            <div>
              <h2>follow us</h2>
            </div>

            <div>
              <img src="../assets/img/footer-facebook.png" alt="">
              <img src="../assets/img/footer-twitter.png" alt="">
              <img src="../assets/img/footer-youtube.png" alt="">
              <img src="../assets/img/footer-pinterest.png" alt="">
              <img src="../assets/img/footer-periscope.png" alt="">
            </div>


          </div>

        </div>

    </div>

  </footer>
  
</template>

<script>
export default {
  name: "FooterComponent"
}
</script>

<style lang="scss" scoped>

@import "../assets/style/variable";

  footer{

    //Top footer

    .top-footer-background{
      height: 400px;
      position: relative;

        .top-footer-content{
          position: relative;
          display: flex;
          width: 80%;
          height: 100%;
          margin: 0 auto;
          color: white;

        }

          .top-footer-content-links{
            display: flex;
            width: 50%;
            height: 100%;
            padding: 20px 0;

            .column-footer-links{
              width: 166px;
              height: 100%;

              h3{
                text-transform: uppercase;
                margin-top: 25px;
                margin-bottom: 10px;
              }

              a{
                font-size: 12px;
                color: gray;
                text-decoration: none;

              }

              li{
                list-style: none;
                margin-bottom: 2px;

              }


            }

          }

          .top-footer-content-dc-background{
            width: 50%;
            background-image: url("../assets/img/dc-logo-bg.png");
            background-position: center center; 
            background-repeat: no-repeat no-repeat;

          }

      

    }

    .top-footer-background::before{
          content: "";
          position: absolute;
          top: 0; left: 0;
          width: 100%; height: 100%;
          background-image: url("../assets/img/jumbotron.jpg");
          filter: brightness(20%);
        }


    //Bottom footer
    
    .bottom-footer{
      background-color: #303030;
      height: 100px;


      .bottom-footer-content{

        display: flex;
        justify-content: space-between;
        align-items: center;

        width: 80%;
        height: 100%;
        margin: 0 auto;


        button{
          padding: 10px;
          border: 2px solid $primary-color;
          text-transform: uppercase;
          background-color: #303030;
          color: white;
          cursor: pointer;
        }


        .social-container{
          display: flex;
          justify-content: center;
          align-items: center;


          h2{
          color: $primary-color;
          text-transform: uppercase;
          margin-right: 30px;
          font-size: 20px;
          }

          img{
          margin-right: 15px;
          cursor: pointer;
          }


        }



      }




    }


  }


</style>