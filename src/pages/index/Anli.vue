<template>
  <Carousel autoplay v-model="value2" loop>
    <CarouselItem>
      <div class="pic-wrap">1</div>
    </CarouselItem>
    <CarouselItem>
      <div class="pic-wrap">2</div>
    </CarouselItem>
    <CarouselItem>
      <div class="pic-wrap">3</div>
    </CarouselItem>
    <CarouselItem>
      <div class="pic-wrap">4</div>
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
<style scoped>
  .pic-wrap{
    width: 100%;
    height: 600px;
    background: #2c3e50;
  }
</style>
