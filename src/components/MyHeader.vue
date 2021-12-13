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

    <!-- jumbotron  -->
    <div>
      <!-- navbar -->
      <nav></nav>
      <!-- /navbar -->
    </div>

    <!-- Banner Get Quote  -->
    <div></div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
$green: #6abf17;
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
</style>
