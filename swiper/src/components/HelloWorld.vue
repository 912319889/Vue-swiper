<template>
  <div class="hello">

    <swiper class="swiper" :options="swiperOption"  ref="mySwiper" style="height: 200px;">
      <!-- slides -->
      <swiper-slide> I'm slide</swiper-slide>
      <swiper-slide> I'm slide 2</swiper-slide>
      <swiper-slide> I'm slide 3</swiper-slide>
      <swiper-slide> I'm slide 4</swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>

  </div>
</template>

<script>
  import 'swiper/dist/css/swiper.css'
  import { swiper, swiperSlide } from 'vue-awesome-swiper'
  export default {
    data(){
      return {
        //设置属性
        swiperOption:{
          //显示分页
          pagination: {
            el: '.swiper-pagination',
          },
        }
      }
    },
    components:{
      swiper,
      swiperSlide
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
