<template>
<div class="jumbotron">
  <div class="jumbotron-top">
    <div class="my-container d-flex position-relative align-items-center justify-content-between">
      <div class="img-background position-absolute">
        <img src="../assets/fable/images/slider_icon16.png" alt="">
        <img class="jumbo-item-down" src="../assets/fable/images/slider_icon14.png" alt="">
        <img src="../assets/fable/images/slider_icon11.png" alt="">
        <img class="jumbo-item-down" src="../assets/fable/images/slider_icon12.png" alt="">
        <img src="../assets/fable/images/slider_icon13.png" alt="">
      </div>
      <div class="jumbo-text">
        <h2>Friendly Atmosphere</h2>
        <h1 class="fw-bold">Welcoming Place</h1>
        <h1 class="fw-lighter">For Every Child</h1>
        <button class="btn btn-warning text-uppercase text-white">Buy this theme Now</button>
      </div>
      <div class="jumbo-img">
        <img class="position-absolute" id="jumbo-first-img" src="../assets/fable/images/slider_slide2_img1.png" alt="">
        <img class="mt-5" src="../assets/fable/images/slider_slide2_img2.png" alt="">
        <div class="rectangles position-absolute">
          <div class="rectangle border border-2 border-danger mx-2"></div>
          <div class="rectangle border border-2 border-danger mx-2 center"></div>
          <div class="rectangle border border-2 border-danger mx-2 "></div>
        </div>
      </div>
    </div>
  </div>
  <div class="jumbotron-bottom">
    <div class="my-container d-flex align-items-center justify-content-between">
      <h1 class="text-white fw-lighter">How to Enroll Your Child to a Class?</h1>
      <button class="btn btn-outline-light">Learn More ></button>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'indexJumbotron',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";
@import url('https://fonts.googleapis.com/css2?family=Indie+Flower&display=swap');
.jumbotron{
  height: 630px;
  .jumbotron-top{
    background-image: url('../assets/fable/images/slider_slide2_background.png');
    background-position: bottom;
    height: 500px;
    .jumbo-text{
      h2{
        color:$orange;
        font-family: 'Indie Flower', cursive;
      }
      h1{
        color:$violet;
      }
      .btn{
        background-color: $orange;
        border-radius: 0 ;
        margin-top: 40px;
      }
    }
    .my-container{
      height: 500px;
      .img-background{
        left: 27%;
        top: 30px;
        .jumbo-item-down{
          position: relative;
          top:60px;
        }
      }
      .jumbo-img{
        height: 100%;
        img{
          height: 80%;
        }
        .rectangles{
          display: flex;
          left: 43%;
          bottom: 5px;
          .rectangle{
            padding: 6px 25px;
          }
          .center{
            position: relative;
            bottom: 20px;
          }
        }
      }
      #jumbo-first-img{
        right: 22%;
        top: 35px;
        height: 90%;
      }
    }
  }
  .jumbotron-bottom{
      background-color: $violet;
      height: 130px;
      width: 100%;
      .my-container{
        height: 100%;
        .btn{
          border-radius: 0;
        }
      }
    }
}
</style>
