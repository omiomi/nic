<template>
  <Carousel autoplay v-model="value2" loop>
    <CarouselItem>
      <div class="pic-wrap">
        <img src="../../assets/pic/pic1.jpg" alt="nic">
      </div>
    </CarouselItem>
    <CarouselItem>
      <div class="pic-wrap">
        <img src="../../assets/pic/pic2.jpg" alt="nic">
      </div>
    </CarouselItem>
    <CarouselItem>
      <div class="pic-wrap">
        <img src="../../assets/pic/pic1.jpg" alt="nic">
      </div>
    </CarouselItem>
    <CarouselItem>
      <div class="pic-wrap">
        <img src="../../assets/pic/pic2.jpg" alt="nic">
      </div>
    </CarouselItem>
  </Carousel>
</template>
<script>
export default {
  data () {
    return {
      value2: 0
    }
  }
}
</script>
<style lang="scss">
  .pic-wrap{
    width: 100%;
    height: 726px;
    background: #0e0e0f;
    position: relative;
    .ivu-carousel-dots{
      li{
        margin: 0 5px;
      }
    }
    img{
      position: absolute;
      top:0;
      left:50%;
      transform: translateX(-50%);
    }
  }
  .ivu-carousel-dots-inside {
    display: block;
    position: absolute;
    bottom: 40px;
  }
  .ivu-carousel-dots li button{
    width: 26px;
    height: 4px;
  }
</style>
