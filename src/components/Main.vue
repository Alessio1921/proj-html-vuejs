<template>
  <main>
    <!-- section welcome -->
    <section id="welcome" class="text-center mt-5">
      <div class="welcome-top">
        <h1>Welcome to Fable</h1>
        <p>Fable daycar,preschool,and kindergarten</p>
        <img src="../assets/fable/images/header_divider.png" alt=" header divider img">
      </div>
      <div class="welcome-footer">
        <div class="my-container d-flex mt-5">
          <div class="element-circle text-center">
            <div class="circle orange mx-auto">
              <img src="../assets/fable/images/schoolbag_alt.png" alt="schoolbag img">
            </div>
            <div class="element-text">
              <h5>Morbis Etos</h5>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatibus, placeat recusandae, libero adipisci beatae laborum.</p>
            </div>
          </div>
          <div class="element-circle text-center">
            <div class="circle violet mx-auto">
              <img src="../assets/fable/images/stroller_alt.png" alt="stroller img">
            </div>
            <div class="element-text">
              <h5>Congue Gravida</h5>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatibus, placeat recusandae, libero adipisci beatae laborum.</p>
            </div>
          </div>
          <div class="element-circle text-center">
            <div class="circle orange mx-auto">
              <img src="../assets/fable/images/bell_alt.png" alt="bell img">
            </div>
            <div class="element-text">
              <h5>Maecenas Node</h5>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatibus, placeat recusandae, libero adipisci beatae laborum.</p>
            </div>
          </div>
          <div class="element-circle text-center">
            <div class="circle violet mx-auto">
              <img src="../assets/fable/images/globe_alt.png" alt="goble img">
            </div>
            <div class="element-text">
              <h5>Praesent Morbi</h5>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatibus, placeat recusandae, libero adipisci beatae laborum.</p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- section overview -->
    <section id="overview" class="mt-5">
      <div class="my-container d-flex">
        <!-- left part -->
        <div class="left">
          <div class="left-top d-flex">
            <div class="title orange text-white">
              <h6>Overview</h6> 
              <div class="arrow-down"></div>
            </div>
            <div class="title border-bottom border-2 ms-3">
              <h6>Our Mission</h6> 
            </div>
          </div>
          <h3 class="my-5">Our philosophy is learning through play as we offer a stimulating environment for children.</h3>
          <div class="left-bottom">
            <!-- left elements -->
            <div class="element d-flex mb-3">
              <div class="circle orange mx-auto me-3">
                <img src="../assets/fable/images/clock_alt.png" alt="clock img">
              </div>
              <div class="description">
                <h3>Full Day Session</h3>
                <p>Pulvinar est metro liglua blandit maecenas retrum gravida cuprum.Maecenas node estibulum</p>
              </div>
            </div>
            <div class="element d-flex">
              <div class="circle orange mx-auto me-3">
                <img src="../assets/fable/images/diagram_alt.png" alt="diagram img">
              </div>
              <div class="description">
                <h3>Varied Classes</h3>
                <p>Pulvinar est metro liglua blandit maecenas retrum gravida cuprum.Maecenas node estibulum</p>
              </div>
            </div>
          </div>
        </div>
        <div class="right">
          <Carousel />
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import Carousel from './Carousel.vue'
export default {
  name: 'indexMain',
  components: {
    Carousel,
  },
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";
  main{
    #welcome{
      h1{
        color: $violet;
      } 
      .welcome-footer{
        .element-circle{
          margin:0 .8rem;
          .circle.orange{
            background-color: $orange;
          }
          .circle.violet{
            background-color: $violet;
          }
          .circle{
            padding: 70px;
            width: 100px;
            height: 100px;
            border-radius: 50%;
            position: relative;
              img{
                position: absolute;
                height: 40%;
                top: 50%;
                left: 50%;
                transform: translate(-50%,-50%);
              }
          }
          .element-text{
            width: 215px;
            h5{
              color: $violet;
            }
          }
        }
      }
    }
    // overview
    #overview{
      background-color: $white;
      .left{
        width: 50%;
        h3{
          color: $violet;
        }
        .title.orange{
          background-color: $orange;
        }
        .title{
          padding:.5rem 1.5rem;
          .arrow-down{
            width: 0px;
            height: 0px;
            border-left: 10px solid transparent;
            border-right: 10px solid transparent;
            border-top: 10px solid $orange;
            position:relative;
            top: 1rem;
            left: 50%;  
            transform: translateX(-50%);
          }
          h6{
            margin-bottom: 0;
            padding-top: 0.5rem;
          }
        }
        .left-bottom{
          .circle.orange{
            background-color: $orange;
          }
          .circle{
            padding: 20px;
            width: 90px;
            height: 70px;
            border-radius: 50%;
            position: relative;
            img{
              position: absolute;
              height: 40%;
              top: 50%;
              left: 50%;
              transform: translate(-50%,-50%);
            }
          }
          h3{
            color:$violet;
          }
        }
      };
      .right{
        width: 50%;
      }
    }
  }
</style>
