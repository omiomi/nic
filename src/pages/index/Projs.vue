<template>
  <div class="projs-wrap">
    <h2>满足个性化需求的解决方案</h2>
    <div class="projs">
      <div class="proj-item" v-for = "item  in list">
        <img :src="item.bg" alt="nic" class="proj-bg">
        <div class="proj-inner">
          <img :src="item.icon" alt="nic" class="icon">
          <img :src="item.iconHover" alt="nic" class="hover">
          <p class="title">{{item.name}}</p>
          <p class="info" v-html="item.info"></p>
          <a href="#" class="more">查看详情</a>
        </div>
      </div>
      <!--
      <div class="proj-item">
        <img src="../../assets/index/proj-bj1.jpg" alt="nic" class="proj-bg">
        <div class="proj-inner">
          <img src="../../assets/index/proj-icon1.svg" alt="nic" class="icon">
          <img src="../../assets/index/proj-icon1-h.svg" alt="nic" class="hover">
          <p class="title">政府机构</p>
          <p class="info">政府机构政府机构政府机构<br>政府机构政府机构</p>
          <div class="more">查看详情</div>
        </div>
      </div>
      <div class="proj-item">
        <img src="../../assets/index/proj-bj2_1.jpg" alt="nic" class="proj-bg">
        <div class="proj-inner">
          <img src="../../assets/index/proj-icon2.svg" alt="nic" class="icon">
          <img src="../../assets/index/proj-icon2-h.svg" alt="nic" class="hover">
          <p class="title">政府机构</p>
          <p class="info">政府机构政府机构政府机构/<br>政府机构政府机构</p>
          <div class="more">查看详情</div>
        </div>
      </div>
      <div class="proj-item on">
        <img src="../../assets/index/proj-bj3.jpg" alt="nic" class="proj-bg">
        <div class="proj-inner">
          <img src="../../assets/index/proj-icon3.svg" alt="nic" class="icon">
          <img src="../../assets/index/proj-icon3-h.svg" alt="nic" class="hover">
          <p class="title">政府机构</p>
          <p class="info">政府机构政府机构政府机构/<br>政府机构政府机构</p>
          <div class="more">查看详情</div>
        </div>
      </div>
      <div class="proj-item">
        <img src="../../assets/index/proj-bj4.jpg" alt="nic" class="proj-bg">
        <div class="proj-inner">
          <img src="../../assets/index/proj-icon4.svg" alt="nic" class="icon">
          <img src="../../assets/index/proj-icon4-h.svg" alt="nic" class="hover">
          <p class="title">政府机构</p>
          <p class="info">政府机构政府机构政府机构/<br>政府机构政府机构</p>
          <div class="more">查看详情</div>
        </div>
      </div>
      <div class="proj-item">
        <img src="../../assets/index/proj-bj5.jpg" alt="nic" class="proj-bg">
        <div class="proj-inner">
          <img src="../../assets/index/proj-icon5.svg" alt="nic" class="icon">
          <img src="../../assets/index/proj-icon5-h.svg" alt="nic" class="hover">
          <p class="title">政府机构</p>
          <p class="info">政府机构政府机构政府机构/<br>政府机构政府机构</p>
          <div class="more">查看详情</div>
        </div>
      </div>
      -->
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      list: [
        {
          name:"政府机构",
          info:"政务系统，服务系统<br>采集系统，大屏展示系统",
          url:"#",
          bg:"static/pic/index/proj-bj1.jpg",
          icon:"static/pic/index/proj-icon1.svg",
          iconHover:"static/pic/index/proj-icon1-h.svg",
        },
        {
          name:"事业单位",
          info:"学籍系统，成绩分析系统<br>采集系统，大屏展示系统",
          url:"#",
          bg:"static/pic/index/proj-bj2_1.jpg",
          icon:"static/pic/index/proj-icon2.svg",
          iconHover:"static/pic/index/proj-icon2-h.svg",
        },
        {
          name:"企业项目",
          info:"企业管理系统，服务系统<br>采集系统，大屏展示系统",
          url:"#",
          bg:"static/pic/index/proj-bj3.jpg",
          icon:"static/pic/index/proj-icon3.svg",
          iconHover:"static/pic/index/proj-icon3-h.svg",
        },
        {
          name:"学术科研",
          info:"期刊系统，实验数据展示系统<br>采集系统，大屏展示系统",
          url:"#",
          bg:"static/pic/index/proj-bj4.jpg",
          icon:"static/pic/index/proj-icon4.svg",
          iconHover:"static/pic/index/proj-icon4-h.svg",
        },
        {
          name:"社团协会",
          info:"活动管理系统，服务系统<br>采集系统，大屏展示系统",
          url:"#",
          bg:"static/pic/index/proj-bj5.jpg",
          icon:"static/pic/index/proj-icon5.svg",
          iconHover:"static/pic/index/proj-icon5-h.svg",
        }
      ]
    }
  }
}
</script>
<style lang="scss">
  .projs-wrap{
    width: 100%;
    height: 560px;
    background: #f6f6f6;
    box-sizing: border-box;
    padding-top: 50px;
    .projs{
      width: 1280px;
      margin: 40px auto;
      display: flex;
      .proj-item{
        width: 20%;
        height: 370px;
        overflow: hidden;
        position: relative;
        display: flex;
        flex: 1;
        &:after{
          content: "";
          display: block;
          position: absolute;
          background: rgba(0,0,0,0.6);
          top:0;
          bottom: 0;
          left: 0;
          right: 0;
        }
        .proj-bg{
          width: 100%;
          position: absolute;
          left: 0;
          right: 0;
          bottom: 0;
          top:0;
        }
        .proj-inner{
          position: relative;
          z-index: 1;
          width: 100%;
          text-align: center;
          transition: all 0.2s cubic-bezier(0.3, 0.6, 0.7, 1.4);
          img{
            position: absolute;
            top:110px;
            left: 50%;
            transform: translateX(-50%);
            height: 70px;
            transition: all 0.2s cubic-bezier(0.3, 0.6, 0.7, 1.4);
            display: none;
            &.hover{
              display: block;
            }
          }
          .title{
            display: block;
            font-size: 22px;
            color: #fff;
            position: relative;
            top:230px;
            transition: all 0.2s cubic-bezier(0.3, 0.6, 0.7, 1.4);
          }
          .info{
            display: none;
            color: #fff;
            font-size: 15px;
            top:200px;
            position: relative;
          }
          .more{display: none;
            height: 24px;
            width: 68px;
            line-height: 24px;
            font-size: 11px;
            text-align: center;
            position: absolute;
            left: 50%;
            bottom: 40px;
            transform: translateX(-50%);
            color: #fff;
            border: 1px solid rgba(200,200,200,.8);
            box-sizing: border-box;
          }
        }
        &:hover{
          &:after{
            background: rgba(227,145,45,.3);
          }
          .proj-inner{
            img{top:60px;
              display: none;
              &.hover{
                display: block;
              }
            }
            .title{top:170px;}
            .info{display: block;}
            .more{display: block;
              &:hover {
                background: linear-gradient(to bottom right, #bf3432, #f2c53b);
                border: 1px solid rgba(0,0,0,0);
              }
            }
          }
        }
      }
    }
    h2{
      font-size: 26px;
      font-weight: 200;
    }
  }
</style>
