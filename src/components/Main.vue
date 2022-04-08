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
    <section id="overview">
      <div class="my-container d-flex">
        <div class="left">

        </div>
        <div class="right"></div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'indexMain',
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
            width: 250px;
            h5{
              color: $violet;
            }
          }
        }
      }
    }
    // overview
    #overview{
      .left{
        width: 50%;
      };
      .right{
        width: 50%;
      }
    }
  }
</style>
