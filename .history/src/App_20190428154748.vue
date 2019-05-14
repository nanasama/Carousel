<template>
  <div id="app">
      <swiper :imgWidth="750" :imgList="imgList" :initIndex="0" :loop="true" :auto="false" :autoTime="2000"></swiper>
  </div>
</template>

<script>
import swiper from './components/carousel'
export default {
  name: 'app',
  data () {
    return {
      imgList:[
          {
             img:'https://jzfp.online-cmcc.cn:10109/fupinnew/pic/201903/201903121039000301100.png?AWSAccessKeyId=SCE2w5trtbBCCWCEVGY1&Expires=4100688000&Signature=Bo0XPz5FJWpFg0su2qqheVaoJ8g%3D'
          },
          {
             img:'http://lorempixel.com/640/480/people'
          },
          {
             img:'http://lorempixel.com/640/480/business'
          }
      ]
    }
  },
  components:{
      swiper
  }
}
</script>

<style lang="css">
    #app{
        width: 800px;
        margin: 0 auto;
    }
</style>
