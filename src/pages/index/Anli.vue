<template>
  <div class="anli-wrap">
    <div class="anli">
      <h2>行业先进技术</h2>
      <div class="indusWrap">
        <div class="industry">
          <img src="../../assets/pic/kLogo.svg" alt="知识图谱" class="logo">
          <h2 class="tlt">知识图谱</h2>
          <p class="info">将不同数据源的结构化结果，通过实体关联构建统一的“实体-关系”图结构模型，提供统一的知识库与知识图谱，支持跨领域数据链接与发现。</p>
          <img src="../../assets/pic/kPic.svg" alt="知识图谱" class="pic">
        </div>
        <div class="industry">
          <img src="../../assets/pic/aiLogo.svg" alt="人工智能" class="logo">
          <h2 class="tlt">人工智能</h2>
          <p class="info">结合“实体-关系”的结构化图谱与具体场景的业务逻辑，对异构信息进行逻辑检验，结合相关性分析与情感分析，推理出可能的隐含信息。</p>
          <img src="../../assets/pic/aiPic.svg" alt="人工智能" class="pic">
        </div>
        <div class="industry">
          <img src="../../assets/pic/deepLearnLogo.svg" alt="深度学习" class="logo">
          <h2 class="tlt">深度学习</h2>
          <p class="info">针对不同的实体类型与用户行为，提供从总体到局部的可视化展现，帮助用户发现形形色色的关系，洞察全面实时的信息变化，简洁易懂。</p>
          <img src="../../assets/pic/deeplearnPic.svg" alt="深度学习" style="height: 88px;" class="pic">
        </div>
      </div>
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
    height: 400px;
    background: #fff;
    box-sizing: border-box;
    .anli{
      position: relative;
      h2{
        font-size: 26px;
        font-weight: 200;
        position: absolute;
        top:45px;
        width: 100%;
        text-align: center;
      }
      width: 1280px;
      margin: 0 auto;
      height: 450px;
      .indusWrap{
        display: flex;
        justify-content:space-between;
      }
      .industry{
        width:410px;
        height: 162px;
        background: #FFF;
        border: 1px solid rgba(235,235,236,1);
        position: relative;
        margin: 150px 0 0;
        .tlt{
          font-weight: 400;
          top:30px;
          padding: 0 15px;
          text-align: left;
          font-size: 16px;
          color:rgba(59,57,57,1);
        }
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
          position: absolute;
          right: 15px;
          top:50%;
          transform: translateY(-50%);
        }
        .info{
          width: 252px;
          text-align: justify;
          position: absolute;
          top:72px;
          left: 15px;
          color:rgba(59,57,57,1);
        }
      }
    }
  }
</style>
