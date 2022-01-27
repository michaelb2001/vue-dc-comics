<template>
<div class="footer">
  <div class="contenitore uno">

    <div class="container ">
        <div class="elemento_primo_container">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <p>DIGITAL COMICS</p>
        </div>

        <div class="elemento_primo_container">
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <p>DC MERCHANDISE</p>
        </div>

        <div class="elemento_primo_container">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <p>SUBSCRITIONS</p>
        </div>

        <div class="elemento_primo_container">
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
          <p>COMIC SHOP LOCATOR</p>
        </div>

        <div class="elemento_primo_container">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <p>DC POWER VISA</p>
        </div>

    </div>

  </div>

  <div class="contenitore due">

    <div class="container">

      <div class="col">
        <h3>DC COMICS</h3>
        <ul>
          <li><a href="">Characters</a></li>
          <li><a href="">Comics</a></li>
          <li><a href="">Movies</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">Games</a></li>
          <li><a href="">Videos</a></li>
          <li><a href="">News</a></li>
        </ul>

        <h3>SHOP</h3>
        <ul>
          <li><a href="">Shop DC</a></li>
          <li><a href="">Shop DC Collectibles</a></li>
        </ul>
      </div>


      <div class="col">
        <h3>DC</h3>
        <ul>
          <li><a href="">Term of use</a></li>
          <li><a href="">privacy policy</a></li>
          <li><a href="">ad choices</a></li>
          <li><a href="">advertising</a></li>
          <li><a href="">jobs</a></li>
          <li><a href="">subscriptions</a></li>
          <li><a href="">telent workshops</a></li>
          <li><a href="">CPSC certification</a></li>
          <li><a href="">Rating</a></li>
          <li><a href="">shop</a></li>
          <li><a href="">concact us</a></li>
        </ul>
      </div>

      <div class="col">
        <h3>sites</h3>
        <ul>
          <li><a href="">DC</a></li>
          <li><a href="">MAD magazine</a></li>
          <li><a href="">DC kids</a></li>
          <li><a href="">DC universe</a></li>
          <li><a href="">DC power visa</a></li>
        </ul>
      </div>
    </div>


    <img src="../assets/img/dc-logo-bg.png" id="dc_bg" alt="background with dc logo">

  </div>

    <div class="contenitore tre">
      
    <div class="container">
      <a href="#" class="btn">sing-up now!</a>

      <div class="social-network">
        <h5>follow us</h5>

        <a href="#" target="_blank" rel="noopener noreferrer" class="icone_social">
          <img src="../assets/img/footer-facebook.png" alt="facebook link">
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer" class="icone_social">
          <img src="../assets/img/footer-twitter.png" alt="twitter link">
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer" class="icone_social">
          <img src="../assets/img/footer-youtube.png" alt="youtube link">
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer" class="icone_social">
          <img src="../assets/img/footer-pinterest.png" alt="pinterest link">
        </a>
        <a href="#" target="_blank" rel="noopener noreferrer" class="icone_social">
         <img src="../assets/img/footer-periscope.png" alt="periscope link">
        </a>
        
      </div>
    </div>

  </div>


</div>


</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/variables.scss';


.contenitore.uno{
  width: 100%;
  background-color: $thirdColor;
  .container{
    display: flex;
    align-items: center;
    justify-content: space-around;
    min-height: 100px;
    width: 100%;
    padding: 20px;
    background-color: $thirdColor;

    .elemento_primo_container{
      display: flex;
      align-items: center;
      justify-content: start;
      margin: 10px;
      img{
        height: 60px;
      }

      p{
        margin-left: 10px;
        color: $secondaryColor;
      }
    }


  }

  
}

.contenitore.due{
    width: 100%;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    justify-content: space-around;
    .container{
      display: flex;
      align-items: center;
      justify-content: start;
      min-height: 100px;
      width: 100%;
      padding: 20px;
      .col{
        text-align: start;
        align-self: start;
        h3{
            color: $secondaryColor;
            margin:10px;
            text-transform: uppercase;
          }

          ul{
            list-style-type: none;
            text-align: start;
            li{

              a{
                text-decoration: none;
                color: $fourthColor;
                margin: 10px;
                text-transform: capitalize;
              }
            }
          }
      }


    }
  }

#dc_bg{
  height: 300px
}

.contenitore.tre{
  background-color: $mainColor;
  height: calc( 100vh - 640px);
  display: flex;
  align-items: center;
  .container{
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .btn{
      color: $thirdColor;
      padding: 15px;
      border: 2px solid $thirdColor;
      font-size:$font1mezzo;
  
    }

    .social-network{
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: space-around;


      h5{
        color:$thirdColor;
        font-size:$font1mezzo;
      }

      .icone_social{
        img{
          height: 30px;
          color: white;
          margin-left: 10px ;
        }
      }

    }
  }
}



</style>
