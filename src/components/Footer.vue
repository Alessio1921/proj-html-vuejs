<template>
  <footer class="mt-5">
    <div class="my-container">
      <div class="footer-top">
        <div class="indications">
          <h6>45°23'45.6"N 75°40'35.6"W</h6>
          <p>98WF+C9F Nepean, Ottawa, Ontario, Canada</p>
        </div>
        <div class="arrow">
          <img src="../assets/fable/images/entity11 (1).png" alt="arrow img">
          <p>Indicazi...</p>
          </div>
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2801.6583391168533!2d-75.67875118467151!3d45.39606247910018!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x378502a87a61b66f!2s87Q698WF%2BC9!5e0!3m2!1sit!2sit!4v1649673298017!5m2!1sit!2sit" width="1080" height="400" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>
      <div class="footer-bottom mt-5 text-center">
        <div class="our-top text-center">
          <h1>Contact Us</h1>
          <p>Our postal and contact datails</p>
          <img src="../assets/fable/images/header_divider.png" alt=" header divider img">
        </div>
        <div class="squares-container d-flex mt-5">
          <div class="square" v-for="(element,index) in contactList" :key="index">
            <div class="img position-relative">
              <img :src="require(`../assets/fable/images/${element.img}`)" alt="">
            </div>
            <h3 class="my-4">{{element.title}}</h3>
            <p>{{element.text1}}</p>
            <p>{{element.text2}}</p>
            <p><a href="#">{{element.text3}}</a></p>
          </div>
        </div>
        <div class="form mt-5 d-flex">
          <div class="left px-3">
            <input type="text" placeholder="Your Name *">
            <input type="email" placeholder="Your E-mail *">
            <input type="text" placeholder="Subject">
          </div>
          <div class="right px-3">
            <textarea name="message" cols="30" rows="10" placeholder="Your Message *"></textarea>
          </div>
        </div>
        <div class="text-center mb-5">
          <button class="btn text-uppercase text-white">Send Message</button>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'indexFooter',
  data:function(){
    return{
      contactList:[
        {
          title:"Postal Address",
          img:"envelope (1).png",
          text1:"Fable Care Canter",
          text2:"85 Fentiman Ave",
          text3:"Ottawa, ON K1S 0T7"
        },
        {
          title:"Phone & E-Mail",
          img:"mobile.png",
          text1:"Phone:1-800-64-38",
          text2:"Fax:1-800-64-39",
          text3:"Office@fable.com"
        },
        {
          title:"Bussines Hours",
          img:"clock.png",
          text1:"Monday-Friday",
          text2:"8.00 am - 5.00 pm",
          text3:"Weekend Closed"
        },
        {
          title:"Sessions",
          img:"document (1).png",
          text1:"Mornings,8 am - 12 noon",
          text2:"Afternoons, 1 pm - 5 pm",
          text3:"Full Day, 8 am - 5 pm"
        }
      ],
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import "../assets/scss/style.scss";
  h1{
    color: $violet;
  }
  .footer-top{
    position: relative;
    .indications{
      position: absolute;
      width: 183px;
      height: 60px;
      z-index: 3;
      background-color: white;
      top: 36px;
      left: 10px;
      h6,p{
        padding-top: 5px;
        padding-left: 15px;
        font-size: .7rem;
        margin: 0;
      }
    }
    .arrow{
      text-align: center;
      background-color: white;
      position: absolute;
      height: 86px;
      width: 50px;
      top:10px;
      left:192px ;
      p{
        color: #1a73e8;
        font-size: .7rem;
        margin-top: .2rem;
      }
    }
  }
  .footer-bottom{
    .square{
      margin: 0 2rem;
      width: calc(100% / 4);
    }
    .form{
      height: 185px;
    }
    .squares-container{
      p{
        margin-bottom: 0;
      }
      h3{
        color: $violet;
      }
      a{
        text-decoration: none;
        color: grey;
        cursor: default;
      }
      .square:nth-child(2){
        a{
          color: $violet;
          cursor: pointer;
          text-decoration: underline;
        }
      }
    }
    .left,
    .right{
      width: 50%;
      input,textarea{
        width: 100%;
        margin: .8rem 0;
        border-radius: 0;
        border: solid $grey;
      }
      textarea{
        height: 75%;
      }
    }
    .btn{
      background-color: $orange;
      border-radius: 0;
    }
  }
</style>
