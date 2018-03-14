<template>
  <div class="header-wrap">
    <div class="nic-header">
      <div class="logo">
        <img src="../assets/img/logo.svg" alt="新智图表">
      </div>
      <ul>
        <li class="on">首页</li>
        <li>可视化图表
          <div class="sub-nav">
            <span class="item"></span>
          </div>
        </li>
        <li>服务行业</li>
        <li>解决方案</li>
        <li>商务合作</li>
        <li>关于我们</li>
      </ul>
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
  .header-wrap{
    width: 100%;
    height: 60px;
    position: fixed;
    top:0;
    z-index: 111;
    background: rgba(0,0,0,.8);
    box-shadow: 1px 1px 1px rgba(0,0,0,.3);
    .nic-header{
      width: 1280px;
      position: absolute;
      left:50%;
      z-index: 100;
      transform: translateX(-50%);
      .logo{
        position: absolute;
        left:0;
        top:6px;
        height: 48px;
        img{
          height: 48px;
          cursor: pointer;
        }
      }
      ul{
        position: absolute;
        left:410px;
        list-style: none;
        line-height: 60px;
        li{
          display: inline-block;
          padding: 0 20px;
          position: relative;
          cursor: pointer;
          font-size: 16px;
          color: #fff;
          &.on,
          &:hover{
            color: #ff9744;
          }
        }
      }
    }
  }
</style>
