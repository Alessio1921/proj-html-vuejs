<template>
  <footer class="mt-5">
    <div class="my-container">
      <div class="footer-top">
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2801.6520383165916!2d-75.6777691284267!3d45.39618956527362!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x7b6d08525cdd95a7!2s87Q698WF%2BF9!5e0!3m2!1sen!2sit!4v1649668935266!5m2!1sen!2sit" width="1080" height="400" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
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
            <p>{{element.text3}}</p>
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
      .square:nth-child(2){
        p:nth-child(5){
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
