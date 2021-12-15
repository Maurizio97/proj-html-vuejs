<template>
  <section>
    <h3 class="sub-title">
        WE ARE A PROFESSIONAL
    </h3>
    <h2 class="title">
        Full&ndash;Service Solution
    </h2>
    <div id="container-card" class="center">
      <!-- card -->
      <!-- <div class="bg-card" > -->
        <div class="card" v-for="item in elSection4" :key="item.title">
          <img :src="item.image" :alt="item.name">
          <div id="cont-text">
            <h2 class="title-card">
            {{ item.name }}
            </h2>
            <p class="text-par">
              "{{ item.paragraph }}"
            </p>
          </div>
        </div>
      <!-- </div> -->
    </div>
    <div id="cont-button">
      <button>READ MORE TESTIMONIALS</button>
    </div>
  </section>
</template>

<script>
export default {
  name: 'MySection4',
  data() {
    return {
      elSection4: [
        {
          image: require("@/assets/img/avada-movers-johndoe-final.jpg"),
          name: "John Doe",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius voluptatem necessitatibus enim. Rerum facilis ipsum, dignissimos dolorum, aliquid ipsa nemo at omnis sint esse saepe explicabo repellat amet illo molestias?",
        },
        {
          image: require("@/assets/img/avada-movers-janedoe-final.jpg"), 
          name: "Jane Doe",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius voluptatem necessitatibus enim. Rerum facilis ipsum, dignissimos dolorum, aliquid ipsa nemo at omnis sint esse saepe explicabo repellat amet illo molestias?",
        },
        {
          image: require("@/assets/img/avada-movers-johnsmith-final.jpg"), 
          name: "Jonh Smith",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius voluptatem necessitatibus enim. Rerum facilis ipsum, dignissimos dolorum, aliquid ipsa nemo at omnis sint esse saepe explicabo repellat amet illo molestias?",
          btn: "READ MORE",
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '@/assets/_variables.scss';

section {
  padding: 150px 0;
  background-image: url("../../src/assets/img/avada-movers-testimonial-background.jpg");
  background-position: right;
  background-size: 120%;
}

.sub-title {
  text-align: center;
}

.title {
  text-align: center;
}

#container-card {
  display: flex;
  justify-content: space-between;

  .card {
    width: calc(100% / 3);
    margin: 60px 0 30px;
    text-align: center;

    img {
      border-radius: 50%;
      height: 150px;
    }
  }
}


#cont-text {
  padding: 40px;
  margin-top: 30px;
}

.title-card {
  color: $blue;
  font-weight: 700;
  font-size: 30px;
}

.text-par {
  margin: 30px auto;
  font-style: oblique;
}

#cont-button {
  margin: 0 auto;
  text-align: center;
}

</style>
