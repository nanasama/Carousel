
/*
 * @Author: zengna 
 * @Date: 2019-05-14 09:56:30 
 * @Last Modified by: ZY.zengna
 * @Last Modified time: 2019-05-14 10:00:50
 */
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
