<template>
  <div id="app">
    <MyHeader :menuItems="navBar"/>
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
  },
  data(){
    return {
      navBar: [
        {
          navItem: "Home"
        },
        {
          navItem: "Rates"
        },
        {
          navItem: "Testimonials"
        },
        {
          navItem: "FAQ"
        },
        {
          navItem: "Blog"
        },
        {
          navItem: "Contact"
        },
      ]
    }
  }
}
</script>

<style lang="scss">
$blue: #1b74c3;
$green: #6abf17;
$colorButton: #1775bf;
$colorSubTitle: #6b6b6b;
#app {
  font-family:  Arial, Helvetica, sans-serif;
  text-align: end;
}

// regole generali
* {
  margin: 0 auto;
  padding: 0 ;
  box-sizing: border-box;
}

.center {
  margin: 0 auto;
  width: 80%;
}

.bg-green {
  background-color: $green;
} 

button {
  background-color: $blue;
  font-size: 15px;
  font-weight: bold;
  color: white;
  padding: 10px 20px;
  border-radius: 20px;
  border: none;
}

</style>
