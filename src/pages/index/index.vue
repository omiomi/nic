<template>
  <div class="index-wrap">
    <Carousel></Carousel>
    <Indus></Indus>
    <Projs></Projs>
    <Anli></Anli>
    <Dingz></Dingz>
  </div>
</template>

<script>
import Carousel from './Carousel'
import Indus from './Indus'
import Projs from './Projs'
import Anli from './Anli'
import Dingz from './Dingz'

export default {
  components: {
    Carousel,
    Indus,
    Projs,
    Anli,
    Dingz
  }
}
</script>

