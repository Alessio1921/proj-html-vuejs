<template>
  <header >
    <div class="my-container">
      <div class="row ">
        <div class="col-12 d-flex justify-content-between">
          <div class="header-logo ">
            <img src="../assets/fable/images/logo.png" alt="logo heaader img">
          </div>
          <div class="right-header">
            <ul class="list-unstyled d-flex">
              <li class="element-header p-4 text-center" :class="(element.active) ? 'active' : ''" v-for="(element,index) in headerList" :key="index">
                <img :src="require(`../assets/fable/`+element.imgActive)" :alt=" element.text+' img'" v-if="element.active">
                <img :src="require(`../assets/fable/`+element.img)" :alt="element.text+' img'" v-else>
                <p>{{element.text}}</p>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'indexHeader',
  props: {
  },
  data:function(){
    return{
      headerList:[
        {
          text:"Home",
          active:true,
          img:"home.png",
          imgActive:"home-2.png",
        },
        {
          text:"Pages",
          active:false,
          img:"document.png",
          imgActive:"document-2.png",
        },
        {
          text:"Blog",
          active:false,
          img:"printer.png",
          imgActive:"printer-2.png",
        },
        {
          text:"Shop",
          active:false,
          img:"cart.png",
          imgActive:"cart-2.png",
        },
        {
          text:"Shortcodes",
          active:false,
          img:"lab.png",
          imgActive:"lab-2.png",
        },
        {
          text:"Support",
          active:false,
          img:"chat.png",
          imgActive:"chat-2.png",
        },
        {
          text:"Contact",
          active:false,
          img:"envelope.png",
          imgActive:"envelope-2.png",
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";
.my-container,
.row,
.col-12,
.header-logo{
  height: 100px;
}
header{
  height: 100%;
  .my-container{
    .row{
      .col-12{
        overflow: hidden;
        .header-logo{
          img{
            height: 100%;
          }
        }
        ul{
          li.active{
            background-color: $orange;
            color: white;
          }
        }
      }
    }
  }
}
</style>
