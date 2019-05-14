<template>
  <div id="app">
      <swiper :imgWidth="750" :imgList="imgList" :initIndex="0" :loop="true" :auto="true" :autoTime="2000"></swiper>
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
             img:'http://lorempixel.com/640/480/transport'
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
