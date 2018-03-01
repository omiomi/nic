<template>
  <div class="dz-wrap">
    <h2>量身定制您的专属数据解决方案</h2>
    <a href="#" class="dz-btn">定制方案</a>
  </div>
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
  .dz-wrap{
    width: 100%;
    height: 318px;
    background: #131914;
    box-sizing: border-box;
    padding-top: 106px;
    h2{
      font-size: 36px;
      color: #fff;
      font-weight: 200;
    }
    .dz-btn{
      font-size: 20px;
      display: inline-block;
      width: 228px;
      height: 46px;
      line-height: 46px;
      margin-top: 20px;
      color: #fff;
      background: linear-gradient(to bottom right, #bf3432, #f2c53b);
      border-radius: 12px;
      &:hover{
        background: linear-gradient(to bottom right, #f2c53b, #bf3432);
      }
    }
  }
</style>
