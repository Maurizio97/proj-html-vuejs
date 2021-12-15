<template>
  <section>
      <div id="cont-for-position" class="center">
          <div class="container-text">
              <h3 class="sub-title">
                WE REMOVE THE HEADACHE FROM MOVING
              </h3>
              <h2 class="title">
                Move With Ease
              </h2>
              <div class="row"></div>
              <p class="text-par">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia eum veritatis voluptatibus nisi provident deleniti sequi voluptas earum cumque, tempora similique doloremque ipsam. Hic, neque.
              </p>
              <button>GET A FREE QUOTE NOW</button>
          </div>
      </div>
  </section>
</template>

<script>
export default {
  name: 'MySection3',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '@/assets/_variables.scss';

section {
  color: white;
  position: relative;
  background-image: url("../../src/assets/img/avada-movers-movewithease-background-new.jpg");
  height: 90vh;
  background-size: 100%;

  #cont-for-position {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: flex-end;
  }

  .container-text {
    width: 40%;
    border: solid 20px green;
    background-color: $green;
    text-align: center;
    padding: 30px;

    .title {
      color: white;
    }

    .sub-title {
      color: white;
      margin: 20px auto 0;
    }

    .row {
      border: solid 1px #79d122;
      width: 80%;
      margin: 20px auto;
    }

    .text-par {
      margin: 20px auto 35px;
    }
  }
}


</style>
