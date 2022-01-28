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

      <div class="colonna">
        <h3>DC COMICS</h3>
        <ul>
          <li v-for="(element,index) in dc_comics" :key="index">
            <a href="">{{element.name.toLowerCase()}}</a>
          </li>

        </ul>

        <h3>SHOP</h3>
        <ul>
          <li v-for="(element,index) in shop" :key="index">
            <a href="">{{element.name.toLowerCase()}}</a>
          </li>
        </ul>
      </div>


      <div class="colonna">
        <h3>DC</h3>
        <ul>
>         <li v-for="(element,index) in dc" :key="index">
            <a href="">{{element.name.toLowerCase()}}</a>
          </li>
        </ul>
      </div>

      <div class="colonna">
        <h3>sites</h3>
        <ul>
>         <li v-for="(element,index) in sites" :key="index">
            <a href="">{{element.name.toLowerCase()}}</a>
          </li>
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
    data(){
    return {
      dc_comics : [
        {
          name : "CHARACTERS",
        },
        {
          name : "COMICS",
        },
        {
          name : "MOVIES",
        },
        {
          name : "TV",
        },
        {
          name : "GAMES",
        },
        {
          name : "COLLECTIBLES",
        },
        {
          name : "VIDEO",
        },
        {
          name : "FANS",
        },
        {
          name : "NEWS",
        }
        
      ],
      shop : [
        {
          name : "Shop DC",
        },
        {
          name : "Shop DC collectibles",
        }
      ],

      dc : [
        {
          name : "term of use",
        },
        {
          name : "privacy policy",
        },
        {
          name : "ad chioces",
        },
        {
          name : "advertising",
        },
        {
          name : "jobs",
        },
        {
          name : "subscritions",
        },
        {
          name : "talent workshop",
        },
        {
          name : "CPSC CERTIFICATION",
        },
        {
          name : "rating",
        },
        {
          name : "shop",
        },        
        {
          name : "contact us",
        }
        
      ],

      sites : [
        {
          name : "DC",
        },
        {
          name : "MAD magazine",
        },
        {
          name : "DC Kids",
        },
        {
          name : "Dc universe",
        },        
        {
          name : "DC power Visa",
        }
      ]


    }
  }
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
      justify-content: space-around;
      min-height: 100px;
      width: 100%;
      padding: 20px;
      .colonna{
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
