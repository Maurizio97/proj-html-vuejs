<template>
  <header>
    <!-- banner Contacts -->
    <div class="bg-green">
      <div class="center" id="cont-banner-contacts">
        <span>
          <i class="fas fa-phone icon"></i>
          Call us for a free quote&colon; &#49;&period;&#56;&#48;&#48;&period;&#53;&#53;&#53;&period;&#54;&#55;&#56;&#57;
        </span>
        <div>
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
      <div id="content-jumbo">
        <!-- navbar -->
        <nav></nav>
        <!-- /navbar -->
      </div>
    </div>

    <!-- Banner Get Quote  -->
    <div id="banner-get-quote">

    </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// varibili colori
$green: #6abf17;
$blueBanner: #1b74c3;

// banner contatti
#cont-banner-contacts {
  height: 45px;
  color: white;
  font-size: 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;

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
}

// banner get quote
#banner-get-quote {
  height: 100px;
  background-color: $blueBanner;
}
</style>
