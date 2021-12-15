<template>
  <footer class="bg-green">
    <!-- top footer -->
    <div id="bg-top-footer">
      
      <!-- contenitore per la parte alta del footer -->
      <div id="top-footer" class="center">

        <!-- colonna 1 -->
        <div class="col-ft">
          <h3>
            ABOUT
          </h3>
          <p class="text-par">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Modi enim delectus veritatis impedit blanditiis natus. Aperiam impedit non magnam, quam ipsa eos officiis tempora quibusdam, a explicabo accusamus facere odio!
          </p>
          <img id="logo-ft" src="../assets/img/avada-movers-logo.png" alt="logo">
        </div>

        <!-- colonna 2 e 3-->
        <ColNavFt 
        v-for="object, i in ArrCont"
        :key="i"
        :contentCol="object"
        />
      </div>
      <!-- /contenitore per la parte alta del footer -->
    </div>
    <!-- /top footer -->

    <!-- bottom footer -->
    <div id="bottom-footer">
      <!-- testo  -->
      <div id="text-bt-ft">
        &copy; Copyright &#50;&#48;&#49;&#50; - &#50;&#48;&#50;&#48; &vert; Avada Theme by ThemeFusion &vert; All Rights Reserved &vert; Powered by WordPress
      </div>

      <!-- icone social -->
      <div id="social-icons-ft">
          <span class="icon"><i class="fab fa-facebook-f"></i></span>
          <span class="icon"><i class="fab fa-twitter"></i></span>
          <span class="icon"><i class="fab fa-instagram"></i></span>
          <span class="icon"><i class="fab fa-youtube"></i></span>
        </div>
    </div>
    <!-- /bottom footer -->
  </footer>
</template>

<script>
import ColNavFt from '../components/ColNavFt.vue'

export default {
  name: 'MyFooter',
  components: {
    ColNavFt,
  },
  props: {
    ArrCont:Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import '@/assets/_variables.scss';

footer {
  padding-top: 25px ;

  #bg-top-footer {
    background-color: white;
  }

  // top footer
  #top-footer {
    display: flex;

    .col-ft {
      width: calc(100% / 3);
      padding: 30px;
      
      // titolo
      h3 {
        margin: 20px 0 25px;
      }
      
      // stile lista
      ul {
        list-style: none;

        li {
          margin: 30px 0 30px;

          a {
            text-decoration: none;
            color: black;
          } 

          .active {
            color: $green;
          }
        }
      }

      #logo-ft {
        margin-top: 25px;
      }
    }
  }
  // /top footer

  // bottom footer
  #bottom-footer {
    color: white;
    padding-bottom: 25px;
  }

  #text-bt-ft {
    text-align: center;
    margin: 25px 0 ;
  }

  #social-icons-ft {
    text-align: center;
  }

  .icon {
    margin: 0 14px;
    font-size: 30px;
  }
}
</style>
