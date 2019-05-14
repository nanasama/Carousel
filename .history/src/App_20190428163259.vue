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
             img:'http://www.jq22.com/img/cs/500x500-1.png'
          },
          {
             img:'http://www.jq22.com/img/cs/500x300-1.png'
          },
          {
             img:'http://www.jq22.com/img/cs/300x500-1.png'
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
