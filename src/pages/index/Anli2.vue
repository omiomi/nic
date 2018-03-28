<template>
  <div class="anli-wrap">
    <div class="anli">
      <swiper :options="swiperOption">
        <swiper-slide v-for="item in anli">
          <img :src="item.url" >
        </swiper-slide>
        <div class="swiper-pagination" slot="pagination"></div>
      </swiper>
    </div>
  </div>
</template>
<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  data () {
    return {
      value2: 0,
      swiperOption: {
        effect: 'coverflow',
        autoplay: {
          delay: 2500,
          disableOnInteraction: false
        },
        loop: true,
        grabCursor: true,
        centeredSlides: true,
        slidesPerView: 'auto',
        coverflowEffect: {
          rotate: 50,
          stretch: 0,
          depth: 400,
          modifier: 1,
          slideShadows : true
        },
        pagination: {
          el: '.swiper-pagination'
        }
      },
      anli: [
        {
          name: 'daping1',
          url: '../../../static/pic/index/anli/dp1.png'
        },
        {
          name: 'daping2',
          url: '../../../static/pic/index/anli/dp5.png'
        },
        {
          name: 'daping1',
          url: '../../../static/pic/index/anli/dp6.jpg'
        }
      ]
    }
  },
  components: {
    swiper,
    swiperSlide
  }
}
</script>
<style lang="scss">
  .anli-wrap{
    width: 100%;
    height: 650px;
    background: #fff;
    box-sizing: border-box;
    .anli{
      width: 1280px;
      margin: 0 auto;
      height: 650px;
      .swiper-container{
        height: 650px;
        img{
          height: 550px;
          position: relative;
          top:50px;
        }
      }
    }
  }
</style>
