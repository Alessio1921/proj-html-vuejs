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
    <section id="overview" class="my-5 py-5">
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
    <!-- section our classes -->
    <section id="our-classes">
      <div class="our-top text-center">
        <h1>Our Classes</h1>
        <p>Our preschool program has four dedicated classes</p>
        <img src="../assets/fable/images/header_divider.png" alt=" header divider img">
      </div>
      <div class="my-container d-flex">
        <!-- left part -->
        <div class="left me-5">
          <h3 class="my-5">
            We provided four classes with nine to twenty children each aged twelve month to five years of age.
          </h3>
        </div>
        <!-- right part -->
        <div class="right">
          <p class="my-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut vitae impedit quo, corporis ipsam hic beatae labore facere saepe sed quae aliquid voluptate ipsum omnis veniam sequi corrupti. Facere, necessitatibus?
            </p>
        </div>
      </div>
      <div class="my-container">
        <Card />
      </div>
    </section>
    <!-- section education -->
    <section id="education" class="mt-5">
      <div class="my-container d-flex">
        <div class="left">
          <h3>We have been educating children for over fitteen vears. Our goal is to create a place tnat engages each child.</h3>
          <p class="my-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Error molestiae impedit minus natus fugit, at enim. Fuga aliquam laudantium eos totam, numquam soluta aliquid velit quis deserunt nesciunt dolore blanditiis?</p>
          <ul>
            <li>
              <img src="../assets/fable/images/style_1.png" alt="check img" class="me-2"> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </li>
            <li>
              <img src="../assets/fable/images/style_1.png" alt="check img" class="me-2"> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </li>
            <li>
              <img src="../assets/fable/images/style_1.png" alt="check img" class="me-2"> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </li>
            <li>
              <img src="../assets/fable/images/style_1.png" alt="check img" class="me-2"> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </li>
            <li>
              <img src="../assets/fable/images/style_1.png" alt="check img" class="me-2"> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </li>
            <li>
              <img src="../assets/fable/images/style_1.png" alt="check img" class="me-2"> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </li>
          </ul>
        </div>
        <div class="right d-flex flex-wrap">
          <div class="square">
            <div class="img position-relative">
              <img src="../assets/fable/images/toy.png" alt="">
            </div>
            <h3>Learning &#38; fun</h3>
            <p>Praesent modea est gravida node vehicula lactus.</p>
          </div>
          <div class="square">
            <div class="img position-relative">
              <img src="../assets/fable/images/meal.png" alt="">
            </div>
            <h3>Healthy Meals</h3>
            <p>Praesent modea est gravida node vehicula lactus.</p>
          </div>
          <div class="square">
            <div class="img position-relative">
              <img src="../assets/fable/images/school.png" alt="">
            </div>
            <h3>Friendly Place</h3>
            <p>Praesent modea est gravida node vehicula lactus.</p>
          </div>
          <div class="square">
            <div class="img position-relative">
              <img src="../assets/fable/images/shield.png" alt="">
            </div>
            <h3>Children Safety</h3>
            <p>Praesent modea est gravida node vehicula lactus.</p>
          </div>
        </div>
      </div>
    </section>
    <section id="gallery" class="my-5">
      <div class="gallery-top d-flex">
        <img src="../assets/fable/images/gallery_01.jpg" alt="">
        <img src="../assets/fable/images/gallery_02.jpg" alt="">
        <img src="../assets/fable/images/gallery_03.jpg" alt="">
        <img src="../assets/fable/images/gallery_04.jpg" alt="">
      </div>
      <div class="gallery-center d-flex">
        <div class="my-container d-flex align-items-center justify-content-between">
          <h1 class="text-white fw-lighter">See Our Kindergarten Photo Gallery!</h1>
          <button class="btn btn-outline-light text-uppercase rounded-0">view gallery ></button>
        </div>
      </div>
      <div class="gallery-bottom text-white">
        <div class="my-container text-center">
          <div class="quote d-flex justify-content-center">
            <div class="rounded-circle border border-light p-3 my-4">
              <img src="../assets/fable/images/quote_alt.png" alt="quote img">
            </div>
          </div>
          <h2>I have to say that I have 2 children ages 5 and 2 and have used various daycare's in Kindergartens and this is by far the very best I have ever used.</h2>
          <div class="divider mx-auto my-4"></div>
          <h6>Cecil J.Kirk</h6>
          <div class="my-thumbnail mx-auto d-flex justify-content-center">
            <div class="rectangle mx-2" v-for="(n,index) in 6" :key="index"></div>
          </div>
        </div>
      </div>
    </section>
    <section id="new">
      <div class="my-container">
        <div class="our-top text-center">
          <h1>What's New</h1>
          <p>Keep up to date with the latest news</p>
          <img src="../assets/fable/images/header_divider.png" alt=" header divider img">
        </div>
        <div class="card-group my-4">
          <div class="card border-0">
            <p class="my-3">October 03,14</p>
            <div class="img position-relative">
              <img src="../assets/fable/images/blog_09.jpg" class="card-img-top " alt="boy photo">
              <div class="position-absolute number p-2">42</div>
            </div>
            <div class="card-body ">
              <h5 class="card-title">Drawing and Painting Lessons</h5>
              <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
            </div>
            <div class="card-footer bg-white">
              <img src="../assets/fable/images/author.png" alt="author img">
              <span class="mx-3">Anna Brown</span>
              <img src="../assets/fable/images/category.png" alt="category img">
              <span class="mx-3">Events,Fun</span>
            </div>
          </div>
          <div class="card border-0 mx-5">
            <p class="my-3">October 03,14</p>
            <div class="img position-relative">
              <img src="../assets/fable/images/blog_10.jpg" class="card-img-top" alt="boys photo">
              <div class="position-absolute number p-2">19</div>
            </div>
            <div class="card-body">
              <h5 class="card-title">Fall Parents Meeting Day</h5>
              <p class="card-text">This card has supporting text below as a natural lead-in to additional content.</p>
            </div>
            <div class="card-footer bg-white">
              <img src="../assets/fable/images/author.png" alt="author img">
              <span class="mx-3">Anna Brown</span>
              <img src="../assets/fable/images/category.png" alt="category img">
              <span class="mx-3">Events,Fun</span>
            </div>
          </div>
          <div class="card border-0">
            <p class="my-3">September 20,14</p>
            <div class="img position-relative">
              <img src="../assets/fable/images/blog_08.jpg" class="card-img-top" alt="boy smile photo">
              <div class="position-absolute number p-2">22</div>
            </div>
            <div class="card-body">
              <h5 class="card-title">Birthday in Kindergarten</h5>
              <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This card has even longer content than the first to show that equal height action.</p>
            </div>
            <div class="card-footer bg-white">
              <img src="../assets/fable/images/author.png" alt="author img">
              <span class="mx-3">Anna Brown</span>
              <img src="../assets/fable/images/category.png" alt="category img">
              <span class="mx-3">Events,Fun</span>
            </div>
          </div>
        </div>
        <!-- <div class="read-more   position-absolute d-flex">read more </div> -->
        <div class="text-center">
          <button class="btn text-uppercase text-white">Go to blog<img src="../assets/fable/images/slider_next.png" alt="next img"></button>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import Carousel from './Carousel.vue'
import Card from './Card.vue'

export default {
  name: 'indexMain',
  components: {
    Carousel,
    Card
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "../assets/scss/style.scss";
  h3,h1{
    color: $violet;
  }
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
      background-color: $grey;
      .left{
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
        }
      }
    }
    // education
    #education{
      ul{
        list-style: none;
        padding: 0;
        li{
          margin-bottom: .5rem;
        }
      }
      p{
        display: inline-block;
      }
      .right{
        .square{
          width: 50%;
          text-align: center;
          .img{
            height: 50%;
            img{
              position: absolute;
              top: 50%;
              left: 50%;
              transform: translate(-50%,-50%);
            }
          }
        }
      }
    }  
    #gallery{
      .gallery-top{
        img{
          width: calc(100% / 4)
        }
      }
      .gallery-center{
        background-image: url("../assets/fable/images/pattern.png");
        height: 120px;
      }
      .gallery-bottom{
        background-image: url("../assets/fable/images/parallax_02.jpg");
        height: 550px;
        background-position: center;
        background-size: cover;
        padding-top: 4rem;
        .divider{
          border: .8px solid white;
          width: 4rem;
        }
        .my-thumbnail{
          margin: 5rem 0;
        }
        .rectangle{
          width: 4rem;
          height: 1rem;
          border: solid 1px white;
        }
        .rectangle:nth-child(3){
          position: relative;
          bottom: 1.5rem;
        }
      }
    }
    #new{
      .my-container{
        .card-footer{
          span{
            color: grey;
          }
        }
        h5{
          color: $violet;
        }
        .number{
          bottom: 0;
          right: 0;
          background-color: $orange;
          color: white;
        }
        .btn{
          background-color: $orange;
          border-radius: 0;
          padding-top: 0.8rem;
          padding-left: 1.3rem;
          height: 3rem;
          img{
            height: 2rem;
          }
        }
      }
    }
  }
</style>
