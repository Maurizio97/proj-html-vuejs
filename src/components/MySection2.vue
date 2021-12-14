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
        <div class="bg-card" v-for="item in elSection2" :key="item.title">
          <div class="card">
            <img :src="item.image" :alt="item.title">
            <div id="cont-text">
              <h2 class="title-card">
              {{ item.title }}
              </h2>
              <p class="text-par">
                {{ item.paragraph }}
              </p>
              <button>{{ item.btn }}</button>
            </div>
          </div>
        </div>
      </div>
      
  </section>
</template>

<script>
export default {
  name: 'MySection2',
  props: {
    content:Array,
  },
  data() {
    return {
      elSection2: [
        {
          image: require("@/assets/img/avada-movers-serviceonephoto-final.jpg"),
          title: "Two Man Teams",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius voluptatem necessitatibus enim. Rerum facilis ipsum, dignissimos dolorum, aliquid ipsa nemo at omnis sint esse saepe explicabo repellat amet illo molestias?",
          btn: "READ MORE",
        },
        {
          image: require("@/assets/img/avada-movers-servicetwophoto-final.jpg"),
          title: "We Do All The Lifting",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius voluptatem necessitatibus enim. Rerum facilis ipsum, dignissimos dolorum, aliquid ipsa nemo at omnis sint esse saepe explicabo repellat amet illo molestias?",
          btn: "READ MORE",
        },
        {
          image: require("@/assets/img/avada-movers-servicethreephoto-final.jpg"),
          title: "Coast To Coast",
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
}

.bg-card {
  margin: 60px 0;
  width: 30%;
  padding: 30px;
  background-color: $bgCardSection2;

  img {
    width: 100%;
  }
}

#cont-text {
  background-color: white;
  padding: 40px;
  margin-top: 30px;
}

div {
  text-align: center;

  .title-card {
    color: $blue;
    font-weight: 700;
    font-size: 30px;
  }

  p {
    margin: 30px auto;
  }
}
</style>
