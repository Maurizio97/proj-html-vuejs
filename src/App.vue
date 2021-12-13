<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  }
}
</script>

<style lang="scss">
$blueBanner: #5babd9;
$green: #6abf17;
$colorButton: #1775bf;
#app {
  font-family:  Arial, Helvetica, sans-serif;
}

// regole generali
* {
  margin: 0 auto;
  padding: 0 auto;
  box-sizing: border-box;
}

.center {
  margin: 0 auto;
  width: 80%;
}

.bg-green {
  background-color: $green;
} 


</style>
