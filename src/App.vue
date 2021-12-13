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
          navItem: "Home",
          active: true
        },
        {
          navItem: "Rates",
          active: false
        },
        {
          navItem: "Testimonials",
          active: false
        },
        {
          navItem: "FAQ",
          active: false
        },
        {
          navItem: "Blog",
          active: false
        },
        {
          navItem: "Contact",
          active: false
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/_variables.scss';

#app {
  font-family:  Arial, Helvetica, sans-serif;
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
