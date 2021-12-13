<template>
  <header>
    <!-- banner Contacts -->
    <div class="bg-green">
      <div class="center" id="cont-banner-contacts">
        <!-- numero di telefono -->
        <div>
          <i class="fas fa-phone icon"></i>
          Call us for a free quote&colon; &#49;&period;&#56;&#48;&#48;&period;&#53;&#53;&#53;&period;&#54;&#55;&#56;&#57;
        </div>

        <!-- icone social -->
        <div id="social-icons">
          <span class="icon"><i class="fab fa-facebook-f"></i></span>
          <span class="icon"><i class="fab fa-twitter"></i></span>
          <span class="icon"><i class="fab fa-instagram"></i></span>
          <span class="icon"><i class="fab fa-youtube"></i></span>
        </div>
      </div>
    </div>
    <!-- /banner Contacts -->

    <!-- jumbotron  -->
    <div id="jumbotron">
      <img id="bg-jumbotron" src="../assets/img/avada-movers-homeherobackground-final.jpg" alt="immagine di sfondo con scatoloni">

      <!-- contenuto jumbotron -->
      <div id="content-jumbo">
        <!-- navbar -->
        <nav class="center">
          <!-- logo -->
          <div id="logo">
            <img src="../assets/img/avada-movers-logo.png" alt="logo avada movers">
          </div>

          <!-- voci menu-->
          <div id="cont-navbar">
            <ul id="navbar">
              <li v-for="item, i in menuItems" :key="i" > 
                <a href="#" :class="item.active? 'active':''">
                  {{ item.navItem }}
                </a>
              </li>
            </ul>
            <button>Free Quote</button>
          </div>
          
        </nav>
        <!-- /navbar -->
      
      <!-- text jumbotron -->
        <div id="cont-text-jumbo">
          <h3>MOVING WITHOUT THE HASSLE</h3>
          <h1>WE MAKE IT SIMPLE</h1>
          <h3>PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION</h3>
        </div>
      <!-- /text jumbotron -->

      </div>
    </div>
    <!-- /jumbotron  -->


    <!-- Banner Get Quote  -->
    <div id="banner-get-quote">
      <div>
      <i class="far fa-paper-plane"></i>
      GET A FREE QUOTE ONLINE NOW&excl;

      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
  props: {
    menuItems:Array
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// varibili colori
@import '@/assets/_variables.scss';

// banner contatti
#cont-banner-contacts {
  height: 45px;
  color: white;
  font-size: 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  div {
    width: 100%;
  }

  #social-icons {
    text-align: right;
  }
  .icon {
    margin: 0 8px;
    font-size: 16px;
  }
}

// jumbotron 
#jumbotron {
  position: relative;
  height: calc(100vh - 145px);

  #bg-jumbotron {
    width: 100%;
    height: 100%;
  }
}

#content-jumbo {
  position: absolute;
  top: 0px;
  width: 100%;
  height: 100%;
}

// nav bar
nav {
  height: 110px;
  display: flex;
  align-items: center;

  #logo {
    width: 100%;
  }

  #cont-navbar {
    width: 100%;
    display: flex;
    align-items: center;
  }

  #navbar {
    display: flex;
    list-style: none;

    li {
      margin: 20px;

      a {
        text-decoration: none;
        color: black;
        font-weight: 800;
        font-size: 14px;

      }

      .active {
        color: $green;
      }
  }
  }
}
// text jumbotron
#cont-text-jumbo {
  height: calc( 100% - 110px );
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  h1 {
    font-size: 60px;
    font-weight: 900;
  }

  h3 {
    color: $colorSubTitle;
    font-size: 16px;
    margin: 8px 0;
  }
}

// banner get quote
#banner-get-quote {
  height: 100px;
  background-color: $blue;
  color: white;
  text-align: center;
  line-height: 100px;
  font-size: 17px;
}
</style>
