<template>
  <section>
      <div>
          <h2 class="title">
              Request A Free Quote
          </h2>
          <p class="text-par">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia eum veritatis voluptatibus nisi provident deleniti sequi voluptas earum cumque, tempora similique doloremque ipsam.
          </p>
          <button>CLICK HERE</button>
      </div>
  </section>
</template>

<script>
export default {
  name: 'MySection5',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
    background-image: url("../../src/assets/img/avada-movers-request-quote-background.jpg");
}

div {
    text-align: center;
    padding: 150px 0;

    p {
        width: 45%;
        margin: 30px auto;
    }
}
</style>
