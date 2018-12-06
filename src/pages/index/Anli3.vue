<template>
  <div class="anli-wrap">
    <div class="anli">
      <h2>典型案例</h2>
      <swiper :options="swiperOption">
        <swiper-slide>
          <div class="industry">
            <img src="../../assets/pic/aiLogo.svg" alt="人工智能" class="logo">
            <h2 class="tlt">人工智能</h2>
            <p>结合“实体-关系”的结构化图谱与具体场景的业务逻辑，对异构信息进行逻辑检验，结合相关性分析与情感分析，推理出可能的隐含信息</p>
            <img src="../../assets/pic/aiPic.svg" alt="人工智能" class="pic">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="industry">
            <img src="../../assets/pic/aiLogo.svg" alt="人工智能" class="logo">
            <h2 class="tlt">人工智能</h2>
            <p>结合“实体-关系”的结构化图谱与具体场景的业务逻辑，对异构信息进行逻辑检验，结合相关性分析与情感分析，推理出可能的隐含信息</p>
            <img src="../../assets/pic/aiPic.svg" alt="人工智能" class="pic">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="industry">
            <img src="../../assets/pic/aiLogo.svg" alt="人工智能" class="logo">
            <h2 class="tlt">人工智能</h2>
            <p>结合“实体-关系”的结构化图谱与具体场景的业务逻辑，对异构信息进行逻辑检验，结合相关性分析与情感分析，推理出可能的隐含信息</p>
            <img src="../../assets/pic/aiPic.svg" alt="人工智能" class="pic">
          </div>
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
        autoplay: {
          delay: 2500,
          disableOnInteraction: false
        },
        loop: true,
        slidesPerView: 3,
        spaceBetween: 60,
        pagination: {
          el: '.swiper-pagination',
          clickable: true
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
    height: 450px;
    background: #fff;
    box-sizing: border-box;
    .anli{
      position: relative;
      h2{
        font-size: 26px;
        font-weight: 200;
        position: absolute;
        top:30px;
        width: 100%;
        text-align: center;
      }
      width: 1280px;
      margin: 0 auto;
      height: 450px;
      .swiper-container{
        margin: 0 auto;
        height: 450px;
        .swiper-slide{
          width: 240px;
          height: 200px;
          box-shadow: 1px 1px 10px #888888;
          position: relative;
          background: #fff;
          top:160px;
          transform: scale(.98);
          box-reflect: below 0 -webkit-linear-gradient(top,rgba(250,250,250,0),rgba(250,250,250,.0) 30%,rgba(250,250,250,0.3));
          &.swiper-slide-next{
            transform: scale(1.5);
            z-index: 11;
          }
          .industry{
            width:385px;
            height: 158px;
            background: #FFF;
            border: 1px solid rgba(235,235,236,1);
            position: relative;
            .logo{
              width: 56px;
              height: 56px;
              position: absolute;
              top:-28px;
              left: 50%;
              margin-left: -28px;
            }
            .pic{
              width: auto;
              height: 100px;
              position: relative;
              right: 20px;
              top:50%;
              transform: translateY(-50%);
            }
          }
        }
      }
    }
  }
</style>
