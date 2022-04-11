<template>
  <div class="carousel">
    <div class="img-principal position-relative">
      <span v-for="(element,index) in photoList" :key="index">
        <img :class="{'d-block': element.active}" :src="require(`../assets/fable/images/`+element.img)" :alt=" element.text+' img'">
      </span>  
        <div class="slider prev position-absolute" @click="prev()">
          <img class="d-block" src="../assets/fable/images/slider_previous.png" alt="prev img">
        </div>
        <div class="slider next position-absolute" @click="next()">
          <img class="d-block" src="../assets/fable/images/slider_next.png" alt=" netx img">
        </div>
    </div>
    <div class="my-thumbnails d-flex">
      <span v-for="(element,index) in photoList" :key="index">
        <div class="my-thumbnail" :class="{'active': element.active}">
          <img :src="require(`../assets/fable/images/`+element.imgThumb)" :alt=" element.text+' img'">
        </div>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name:"CarouselHome",
  data:function(){
    return{
      counter:2,
      photoList:[
        {
          img:"gallery_07-690x506.jpg",
          active:false,
          text:"little girl photo",
          imgThumb:"gallery_07-690x506.jpg",
        },
        {
          img:"gallery_01-690x506.jpg",
          active:false,
          text:"children photo",
          imgThumb:"gallery_01-690x506.jpg",
        },
        {
          img:"gallery_08-690x506.jpg",
          active:true,
          text:"teacher photo",
          imgThumb:"gallery_08-690x506.jpg",
        }
      ],
    }
  },
  methods:{
    prev(){ 
      if(this.counter==0){
        this.photoList[this.counter].active=false;
        this.counter=this.photoList.length-1;
        this.photoList[this.counter].active=true;
      }
      else{
        this.photoList[this.counter].active=false;
        this.photoList[this.counter-1].active=true;
        this.counter--;
      }
    },
    next(){    
      if(this.counter==this.photoList.length-1){
        this.photoList[this.counter].active=false;
        this.counter=0;
        this.photoList[this.counter].active=true;
      }
      else{
        this.photoList[this.counter].active=false;
        this.photoList[this.counter+1].active=true;
        this.counter++;
      }
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

  .carousel{
    width: 100%;
    .img-principal{
      img{
        width: 100%;
        display: none;
      }
      .slider{
        background-color: $orange;
        top: 50%;
        transform: translateY(-50%);
        cursor: pointer;
      }
      .prev{
        left:0;
      }
      .next{
        right:0;
      }
    }
    .my-thumbnails{
      margin-top: .8rem;
      overflow: hidden;
      width: 100%;
      .my-thumbnail{
        padding-bottom: .5rem ;
        height: 135px;
        width: 100%;
        img{
          height: 100%;
        }
      }
      .my-thumbnail.active{
        border-bottom: 3px solid $orange;
      }
    }
    .my-thumbnails span:nth-child(2){
      margin: 0 .8rem;
    }
  }
</style>