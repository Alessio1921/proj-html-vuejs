<template>
  <div class="d-flex flex-wrap">
    <div class="my-card d-flex" v-for="(element,index) in cardList" :key="index">
      <div class="info p-3">
        <h5 class="text-white">{{element.title}}</h5>
        <p class="text-white">Class name</p>
        <div class="info-bottom position-relative text-center">
          <div class="year text-center pe-3 border-end border-2 border-light d-inline-block">
            <p>{{element.age}}</p>
            <p>{{element.year}}</p>
          </div>
          <div class="size text-center ms-3 d-inline-block">
            <p>{{element.size}}</p>
            <p>Class size</p>
          </div>
        </div>
      </div>
      <div class="img position-relative">
        <img :src="require(`../assets/fable/images/`+element.img)" :alt=" element.text+' img'">
        <button class="btn rounded-0 read-more text-uppercase text-white position-absolute d-flex">read more <img src="../assets/fable/images/slider_next.png" alt="next img"></button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:"CardHome",
  data:function(){
    return{
      cardList:[
        {
          title:"Little Lambs",
          age:"12-24",
          year:"Month olds",
          size:9,
          img:"class_01-690x506.jpg",
          text:"little girl photo",
        },
        {
          title:"Bouncy Bears",
          age:"2-3",
          year:"Year old",
          size:12,
          img:"class_02-690x506.jpg",
          text:"teacher photo",
        },
        {
          title:"Tenderhearts",
          age:"3-4",
          year:"Year old",
          size:15,
          img:"class_03-690x506.jpg",
          text:"little girl photo",
        },
        {
          title:"Shining Star",
          age:"4-5",
          year:"Year old",
          size:20,
          img:"class_04-690x506.jpg",
          text:"children photo",
        }
      ],
    }
  },
}
</script>

<style scoped lang="scss">
  @import "../assets/scss/style.scss";
  .my-card{
    width: 508px;
    height: 175px;
    background-color: $violet;
    margin: 0 2rem 2rem 0;
    .info{
      width: 50%;
      .info-bottom{
        color: white;
        top:50px;
        font-size:.9rem
      }
      p{
        color: white;
        margin: 0;
      }
    }
    .img{
      width: 50%;
      img{
        height: 100%;
        width: 100%;
      }
      .read-more{
        bottom: 0;
        right: 0;
        background-color: $orange;
        padding: .8rem;
        font-size: .8rem;
        padding-top: 0.5rem;
        padding-left: 1rem;
        padding-bottom: 0.2rem;
        font-size: 0.7rem;
        font-weight: bold;
        align-items: center;
        img{
          width: 1.7rem;
        }
      }
    }
  }
</style>