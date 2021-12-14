<template>
  <div id="app">
    <MyHeader :menuItems="navBar"/>
    <MyMain/>
    <MyFooter :itemsAvadaMovers="avadaMovers" :itemsRecentPosts="recentPost"/>
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
      ],
      avadaMovers: [
        {
          name: "Home",
          active: true
        },
        {
          name: "Rates",
          active: false
        },
        {
          name: "Testimonials",
          active: false
        },
        {
          name: "Blog",
          active: false
        },
        {
          name: "Free Quote",
          active: false
        },
      ],
      recentPost: [
        {
          name: "Hendling Out To College&quest;",
          active: false
        },
        {
          name: "Moving Your Business&quest;",
          active: false
        },
        {
          name: "Outstanding Quality",
          active: false
        },
        {
          name: "Cost of Moving",
          active: false
        },
        {
          name: "Best Moving Tips",
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
  padding: 15px 30px;
  border-radius: 20px;
  border: none;
}
.title {
  color: $green;
  font-size: 45px;
  font-weight: 900;
}

.sub-title {
  color: $colorSubTitle;
  font-size: 18px;
}

.text-par {
  line-height: 2;
  font-size: 17px;
}


</style>
