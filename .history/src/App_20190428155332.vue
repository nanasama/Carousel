<template>
  <div id="app">
      <Carousel :imgWidth="750" :imgList="imgList" :initIndex="0" :loop="true" :auto="false" :autoTime="2000"></Carousel>
  </div>
</template>

<script>
import Carousel from './components/carousel'
export default {
  name: 'app',
  data () {
    return {
      imgList:[
          {
             img:'https://jzfp.online-cmcc.cn:10109/fupinnew/pic/201903/201903121039000301100.png?AWSAccessKeyId=SCE2w5trtbBCCWCEVGY1&Expires=4100688000&Signature=Bo0XPz5FJWpFg0su2qqheVaoJ8g%3D'
          },
          {
             img:'https://jzfp.online-cmcc.cn:10109/fupinnew/pic/201902/201902210943000538349.png?AWSAccessKeyId=SCE2w5trtbBCCWCEVGY1&Expires=4100688000&Signature=XE7q46Ne%2B6xG6S7AhM9Qoq6zDEE%3D'
          },
          {
             img:'https://jzfp.online-cmcc.cn:10109/fupinnew/pic/201806/201806072236173513781.png?AWSAccessKeyId=SCE2w5trtbBCCWCEVGY1&Expires=4100688000&Signature=xPwPxwWgEfECRyGUnw85bMs42%2Bg%3D'
          }
      ]
    }
  },
  components:{
      Carousel
  }
}
</script>

<style lang="css">
    body{
          background: #e4eff3;
    }
    #app{
        width: 800px;
        margin: 0 auto;
    }
</style>
