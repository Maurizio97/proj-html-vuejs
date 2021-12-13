<template>
  <header>
    <span>
        ciao sono mario
      <i class="fas fa-phone"></i>
    </span>
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
span {
  color: $green;
  font-size: 100px;
}
</style>
