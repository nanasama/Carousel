<template>
  <div id="app">
      <Carousel :imgWidth="750" :imgList="imgList" :initIndex="0" :loop="true" :auto="true" :autoTime="2000"></Carousel>
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
             img:'http://lorempixel.com/640/480/cats'
          },
          {
             img:'http://lorempixel.com/640/480/nature'
          },
          {
             img:'http://lorempixel.com/640/480/technics'
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
