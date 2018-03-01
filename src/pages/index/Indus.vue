<template>
  <div class="indus-wrap">
    <h2>服务覆盖14个行业</h2>
    <Row type="flex" justify="end" class="indus-row code-row-bg">
      <Col span="3">
        <div class="icon-wrap">
          <img src="../../assets/svg/icon1.svg" alt="生鲜行业">
          <span>生鲜行业</span>
        </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon2.svg" alt="车联网">
        <span>车联网</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon3.svg" alt="物联网">
        <span>物联网</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon4.svg" alt="科技物流">
        <span>科技物流</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon5.svg" alt="科技金融">
        <span>科技金融</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon6.svg" alt="旅游">
        <span>旅游</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon7.svg" alt="互联网医疗">
        <span>互联网医疗</span>
      </div>
      </Col>
    </Row>
    <Row type="flex" justify="end" class="indus-row code-row-bg">
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon8.svg" alt="环保">
        <span>环保</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon9.svg" alt="电子行业">
        <span>电子行业</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon10.svg" alt="智能制造">
        <span>智能制造</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon11.svg" alt="消费金融">
        <span>消费金融</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon12.svg" alt="电子信息">
        <span>电子信息</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon13.svg" alt="教育">
        <span>教育</span>
      </div>
      </Col>
      <Col span="3">
      <div class="icon-wrap">
        <img src="../../assets/svg/icon14.svg" alt="泛娱乐">
        <span>泛娱乐</span>
      </div>
      </Col>
    </Row>
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
  .indus-wrap{
    width: 100%;
    height: 680px;
    background: #fff;
    box-sizing: border-box;
    padding-top: 56px;
    .indus-row{
      width: 1280px;
      height: 140px;
      justify-content: space-around;
      margin: 100px auto 0;
    }
    .icon-wrap{
      position: relative;
      span{
        position: relative;
        top: 80px;
      }
      img{
        position: absolute;
        left:50%;
        top:50%;
        transform: translateX(-50%) translateY(-50%) scale(.5);
      }
    }
    h2{
      font-size: 26px;
    }
  }
</style>
