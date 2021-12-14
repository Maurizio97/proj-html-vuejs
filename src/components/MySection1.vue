<template>
  <section>
      <div>
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
  </section>
</template>

<script>
export default {
  name: 'MySection1',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '@/assets/_variables.scss';

section {
    background-color: $bgCardSection2;
}
div {
    text-align: center;
    padding: 150px 0;

    h2 {
        width: 25%;
        margin: 0 auto;
    }

    p {
        width: 40%;
        margin: 30px auto;
    }
}
</style>
