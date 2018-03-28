<template>
  <div class="footer-wrap">
    <div class="footer">
      <div class="f-item">
        <img src="../assets/img/nic-log.png" alt="nic" class="f-logo">
        <br>
        <span class="f-slogon">
          更美、更艺术、更易用<br>
          爱上图表 爱上NIC
        </span>
      </div>
      <div class="f-item">
        <h2>可视化图表</h2>
        <ul>
          <li>大屏可视化</li>
          <li>Android端可视化</li>
          <li>iOS端可视化</li>
          <li>PC端可视化</li>
          <li>多端互动</li>
        </ul>
      </div>
      <div class="f-item">
        <h2>服务行业</h2>
        <ul>
          <li>服务大数据</li>
          <li>服务人工智能</li>
          <li>服务VR\AR</li>
          <li>服务科技金融</li>
          <li>服务创新创业</li>
        </ul>
      </div>
      <div class="f-item">
        <h2>解决方案</h2>
        <ul>
          <li>中央指挥室</li>
          <li>迎宾大屏</li>
          <li>监控系统</li>
          <li>报警系统</li>
          <li>大屏可视化</li>
        </ul>
      </div>
      <div class="f-item">
        <h2>关于NIC</h2>
        <ul>
          <li>NIC品牌</li>
          <li>NIC博客</li>
          <li>NIC官微</li>
          <li>NIC百科</li>
          <li>加入NIC</li>
        </ul>
      </div>
      <div class="f-item">
        <h2 class="last">关注二维码</h2>
        <img src="../../static/img/ewm.png" alt="nic" class="ewm">
      </div>
      <div class="copyright">
        Copyright©2018 北京新智图表有限公司 | 京ICP备12345678号-8
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      theme1: 'light'
    }
  }
}
</script>
<style lang="scss">
  .footer-wrap {
    width: 100%;
    height: 240px;
    background: #000;
    box-sizing: border-box;
    position: relative;
    .footer{
      width: 1280px;
      margin: 30px auto;
      display: flex;
      .f-item{
        width: 16%;
        text-align: left;
        .f-logo{
          width: 100px;
        }
        .f-slogon{
          font-size: 18px;
        }
        h2{
          font-size: 22px;
          font-weight: 400;
          padding-bottom: 10px;
          position: relative;
          left: 25px;
          &.last{
            left: -5px;
          }
        }
        ul{
          position: relative;
          left: 29px;
          li{
            text-align: left;
          }
        }
        .ewm{
          width: 100px;
          position: relative;
          top:4px;
        }
      }
      .copyright{
        width: 800px;
        padding-top: 10px;
        border-top:1px solid rgba(100,100,100,.3);
        position: absolute;
        bottom: 30px;
        left:50%;
        transform: translateX(-50%);
      }
    }
  }
</style>
