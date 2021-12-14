<template>
  <section>
      <div class="center">
          <div class="container-text">
              <h3 class="sub-title">
              HEADACHE FREE
              </h3>
              <h2 class="title">
                Award Winning Moving Company
              </h2>
              <p class="text-par">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia eum veritatis voluptatibus nisi provident deleniti sequi voluptas earum cumque, tempora similique doloremque ipsam. Hic, neque. Tenetur quod suscipit dolores repellat?
              </p>
              <button>READ OUR TESTIMONIALS</button>
          </div>
      </div>
  </section>
</template>

<script>
export default {
  name: 'MySection3',
    data(){
      return {
          // bgImage: require("@/assets/img/avada-movers-movewithease-background-new.jpg")
      }
    }
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
  
  .container-text {
    width: 40%;
    border: solid 20px green;
    background-color: $green;
    text-align: center;

    .title {
      color: white;
    }

    .sub-title {
      color: white;
    }
  }
}


</style>
