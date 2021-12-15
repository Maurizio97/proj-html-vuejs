<template>
  <!-- colonna 2 -->
  <div class="col-ft">
    <h3>
      {{ contentCol.title.titleName }}
    </h3>
    <ul>
      <li v-for="item in contentCol.nav" :key="item" > 
        <a href="#" :class="item.active? 'active':''">
          <i class="fas fa-chevron-right"></i>
          {{ item.name }}
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'ColNavFt',
  props: {
    contentCol:Object,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
