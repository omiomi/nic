<template>
  <div class="projs-wrap">
    <h2>满足个性化需求的解决方案</h2>
    <div class="projs">
      <Row type="flex" justify="end" class="projs-list code-row-bg">
        <Col span="4">
        <Card :bordered="false">
          <p slot="title">政府机构</p>
          <p>铁道部</p>
          <p>市科委</p>
          <p>发改委</p>
        </Card>
        </Col>
        <Col span="4">
        <Card :bordered="false">
          <p slot="title">事业单位</p>
          <p>医院</p>
          <p>福利社</p>
          <p>邮局</p>
        </Card>
        </Col>
        <Col span="4">
        <Card :bordered="false">
          <p slot="title">企业项目</p>
          <p>阿里巴巴</p>
          <p>高德地图</p>
          <p>微信云</p>
        </Card>
        </Col>
        <Col span="4">
        <Card :bordered="false">
          <p slot="title">学术科研</p>
          <p>传感技术学会</p>
          <p>重点实验室</p>
          <p>基因工程</p>
        </Card>
        </Col>
        <Col span="4">
        <Card :bordered="false">
          <p slot="title">社团协会</p>
          <p>建筑协会</p>
          <p>福利社</p>
          <p>多背一公斤</p>
        </Card>
        </Col>
      </Row>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style lang="scss">
  .projs-wrap{
    width: 100%;
    height: 560px;
    background: #f6f6f6;
    box-sizing: border-box;
    padding-top: 56px;
    .projs{
      width: 1280px;
      margin: 50px auto;
      .projs-list{
        justify-content: space-around;
        .ivu-card{
          height: 340px;
        }
      }
    }
    h2{
      font-size: 26px;
      font-weight: 200;
    }
  }
</style>
