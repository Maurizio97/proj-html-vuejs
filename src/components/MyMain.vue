<template>
  <main>
    <!-- sezione 1 -->
    <MySection1/>
    <!-- sezione 2 -->
    <MySection2 :content="elSection2"/>
    <!-- sezione 5 -->
    <MySection5/>
  </main>
</template>

<script>
import MySection1 from '../components/MySection1.vue'
import MySection2 from '../components/MySection2.vue'
import MySection5 from '../components/MySection5.vue'
export default {
  name: 'MyMain',
  components: {
    MySection1,
    MySection2,
    MySection5,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
