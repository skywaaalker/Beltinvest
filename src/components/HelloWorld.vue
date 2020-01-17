<template>
  <div class="front-page">
    <div class="page-header">
      <img src="@/assets/img/logo@2x.png"/>
      <div class="nav">
        <ul>
          <li><a @click="changeHash('#part-1')">平台介绍</a></li>
          <li><a @click="changeHash('#part-2')">亚洲精选</a></li>
          <li><a @click="changeHash('#part-3')">关于我们</a></li>
        </ul>
      </div>
    </div>
    <div class="float-image">
      <img src="@/assets/img/img_code@2x.png">
      <div class="p-scan-code">扫码投资</div>
    </div>
    <div class="show-img" style="width:100%">
      <img src="@/assets/img/banner@2x.png" style="width:100%;"/>

    </div>
    <div class="mid-part1">
      <div id="part-1" style="position: relative;padding-top: 50px;margin-top: -50px;"></div>
      <div class="mid-part1-box">
        <Title title="平台介绍"></Title>
        <p>印度及东南亚数字经济蓬勃发展，而传统金融服务覆盖率极低，金融科技将引来爆发式增长。</p>
        <p>丝路投资为投资人精选亚洲的优质信贷资产，推出固定期限、固定收益类美元理财产品。</p>
        <p>底层资产小额分散，风险可控，投资标的由信贷运营母公司进行担保，保障投资人本金及收益安全。</p>
        <div class="icon-list">
          <Intropart title="优质资产" subtitle="精选优质借款人，小款分散，风险可控" iconname="zichan">
          </Intropart>
          <Intropart title="安全合规" subtitle="在亚洲各国持续经营,合法合规" iconname="safe">
          </Intropart>
          <Intropart title="风控保障" subtitle="机器学习风控技术，由信贷运营母公司担保" iconname="fengkong">
          </Intropart>
        </div>
      </div>
      <div id="part-2" style="position: relative;padding-top: 50px;margin-top: -50px;"></div>
    </div>
    <div class="mid-part2">
      <div class="mid-part2-box">
        <Title title="亚洲精选"></Title>
        <img src="@/assets/img/plan4@2x.png"/>
        <div class="icon-list">
          <Intropart title="法律风控" subtitle="平台合作个人信贷项目均持牌展开业务，合法合规" iconname="law">
          </Intropart>
          <Intropart title="技术风控" subtitle="强大的工程师团队，采用大数据及机器学习，运用超过2000个数据标签，进行多重风控保障" iconname="jishu">
          </Intropart>
          <Intropart title="资产风控" subtitle="交易结构的设置上，信贷运营方母公司对借款项目进行担保，确保投资人利益" iconname="zichanfengkong">
          </Intropart>
        </div>
      </div>
      <div id="part-3" style="position: relative;padding-top: 50px;margin-top: -50px;"> </div>
    </div>
    <div class="mid-part3">
      <div class="mid-part3-box">
        <Title title="关于我们"></Title>
        <div class="p-box">
        <p>丝路投资平台隶属新加坡Brilliant Foundation，其母公司Black Fish Group由著名企业家创立，已获得包括光速中国、光速美国、晨兴资本、日本乐天、集富亚洲、华创资本、沸点资本、戈壁创投等知名基金的投资。</p>
        </div>
        <div class="leader-list">
        <Leaderintro title="Alex Yan" subtitle="Black Fish Group CEO" leadername="yan"></Leaderintro>
        <Leaderintro title="Conor Yang" subtitle="Black Fish Group President" leadername="yang" ></Leaderintro>
        <Leaderintro title="Frank Li" subtitle="Beltinvest General Manager" leadername="li"></Leaderintro>
        </div>
        <div class="sponsor-list">
          <div class="table">
            <div class="tr">
              <div class="td"><img src="@/assets/img/sponsors/logo_guangsu1@2x.png"></div>
              <div class="td"><img src="@/assets/img/sponsors/logo_guangsu@2x.png"></div>
              <div class="td"><img src="@/assets/img/sponsors/logo_chengxing@2x.png"></div>
              <div class="td"><img src="@/assets/img/sponsors/logo_rakuten@2x.png"></div>
            </div>
            <div class="tr">
              <div class="td"><img src="@/assets/img/sponsors/logo_jifu@2x.png"></div>
              <div class="td"><img src="@/assets/img/sponsors/logo_huachuang@2x.png"></div>
              <div class="td"><img src="@/assets/img/sponsors/logo_feidian@2x.png"></div>
              <div class="td"><img src="@/assets/img/sponsors/logo_gebi@2x.png"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="page-footer">
      <div class="page-footer-box">
        <div class="footer-icon-list">

          <el-popover class="el-popover-distance" placement="top"  width="170" trigger="click" >
            <table border="0">
              <tr>
                <td><img src="@/assets/img/img_code@2x.png" width="80px" height="80px"></td>
                <td><img src="@/assets/img/img_code@2x.png" width="80px" height="80px"></td>
              </tr>
              <tr>
                <td style="text-align: center">客服微信号</td>
                <td style="text-align: center">微信公众号</td>
              </tr>
            </table>
            <el-button  slot="reference" icon="el-icon-chat-dot-round" size="mini" circle ></el-button>
          </el-popover>
          <el-popover class="el-popover-distance" placement="top" title="客服热线" width="210" trigger="click" content="4000-000-0000">
            <el-button slot="reference" icon="el-icon-service" size="mini" circle ></el-button>
          </el-popover>
          <el-popover class="el-popover-distance" placement="top" width="210" trigger="click" >
            <p style="line-height:8px; font-size:12px; color:#666 margin:10px auto;">总部地址</p>
            <p style="line-height:18px; font-size:16px; color:#333">2 VENTURE DRIVE, 11-31, VISION EXCHANGE, SINGAPORE(608526)</p>
            <a style="text-decoration:none; color:#4a90e2; font-size:12px;" href="https://goo.gl/maps/4yneZXGLhxnJ6vLu8" target="_blank">查看地图</a>

            <el-button slot="reference"  icon="el-icon-location-outline" size="mini" circle ></el-button>
          </el-popover>
          <el-popover class="el-popover-distance" placement="top" title="客服邮箱" width="220" trigger="click" content="CustomerSevice@Beltinvest.com">
            <el-button slot="reference" icon="el-icon-message" size="mini" circle ></el-button>
          </el-popover>
          <!-- <img src="@/assets/img/icons/ic_chat@2x.png">
          <img src="@/assets/img/icons/ic_map@2x.png">
          <img src="@/assets/img/icons/ic_email@2x.png">
          <img src="@/assets/img/icons/ic_phone@2x.png"> -->
        </div>
        <p class="font-14">Copyright 2019 - 2020 Brilliant Foundation. All Rights Reserved.</p>
        <p class="font-12">丝路投资平台并不且无意在任何司法区域内向该司法区域内任何人士销售、推广或宣传在该司法区域内不获授权、核准或豁免与规例的任何产品或服务。</p>
      </div>
    </div>
  </div>
</template>

<script>
import Title from './title'
import Intropart from './intropart'
import Leaderintro from './leaderintro'

export default {
  name: 'HelloWorld',
  components: {
    Title,
    Intropart,
    Leaderintro
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      screenWidth: '',
      screenHeight: ''
    }
  },
  mounted () {
    this.$router.afterEach((to, from, next) => {
      window.scrollTo(0, 0)
    })
  },
  methods: {
    changeHash (idName) {
      // var element = document.getElementById(idName)
      // element.scrollIntoView()
      // element.scrollIntoView(true)
      // element.scrollIntoView({behavior: 'smooth'})
      // document.querySelector(idName).scrollIntoView(true)
      // document.querySelector(idName).scrollIntoView({behavior: 'smooth'})
      const targetOffsetTop = document.querySelector(idName).offsetTop
      let scrollTop = document.documentElement.scrollTop || document.body.scrollTop
      const step = 20
      if (scrollTop > targetOffsetTop) {
        smoothUp()
      } else {
        smoothDown()
      }
      function smoothDown () {
        if (scrollTop < targetOffsetTop) {
          if (targetOffsetTop - scrollTop >= step) {
            scrollTop += step
          } else {
            scrollTop = targetOffsetTop
          }
          document.body.scrollTop = scrollTop
          document.documentElement.scrollTop = scrollTop
          requestAnimationFrame(smoothDown)
        }
      }
      function smoothUp () {
        if (scrollTop > targetOffsetTop) {
          if (scrollTop - targetOffsetTop >= step) {
            scrollTop -= step
          } else {
            scrollTop = targetOffsetTop
          }
          document.body.scrollTop = scrollTop
          document.documentElement.scrollTop = scrollTop
          requestAnimationFrame(smoothUp)
        }
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style lang="less" scoped>
.front-page{
  min-height: 100vh;
  margin: 0 auto;
  .page-header{
    height: 70px;
    width: 100%;
    background-color: #fff;
    position:fixed;
    top:0;
    left: 0;
    z-index: 50;
    img{
      float: left;
      margin-left: 70px;
      margin-top: 22px;
      margin-bottom: 0px;
      width: 263px;
      height: 36px;
    }
    .nav{
      float: left;
      height: 80px;
      text-align: center;
      ul{
        padding-top: 30px;
        padding-bottom: 30px;
        list-style: none;
        width: 400px;
        overflow: hidden;
        margin: 0;
        li{
          padding-left: 60px;
          text-align: center;
          float: left;
          width: 64px;
          font-size: 16px;
          font-family: Microsoft YaHei;
          a{
            text-decoration: none;
          }
          a:link{
            color:#333;
          }
          a:visited{
            color:#333;
          }
          a:hover{
            color:#c99d55;
          }
          a:active{
            color:#c99d55;
          }
        }
      }
    }
  }
  .float-image{
    z-index: 999;
    position: fixed;
    right: 50px;
    top: 20px;
    width: 110px;
    height: 125px;
    background-color: #fff;
    img{
      width: 100px;
      height: 100px;
    }
    .p-scan-code{
      text-align: center;
      margin: 0 auto;
      font-size: 15px;
      letter-spacing: 7px;
      line-height: 10px;
    }
  }
  .show-img{
    width:100%;
    position: relative;
    margin-top: 80px;
    .img{
      margin: 0;
      padding: 0;
      position: absolute;
      width:100%;
      height: 100%;
    }
  }
  .mid-part1{
    width: auto;
    margin-top: 10px;
    .mid-part1-box{
      width: 70%;
      margin-top: 49px;
      display: inline-block;
      Title{
      }
      p{
        margin-top: 15px;
        font-size: 14px;
        color: #999;
        line-height: 12px;
      }
      .icon-list{
        height: 200px;
        width: 100%;
      }
    }

  }
  .mid-part2{
    width: auto;
    background-color: #f9f9f9;
    padding-top: 49px;
    .mid-part2-box{
      width: 70%;
      display: inline-block;
      Title{
      }
      img{
        margin-top: 18px;
        width: 677px;
        height: 248px;
      }
      .icon-list{
        height: 200px;
        width: 100%;
      }
    }
  }
  .mid-part3{
    width: auto;
    background-color: #ffffff;
    padding-top: 49px;
    .mid-part3-box{
      width: 100%;
      display: inline-block;
      .p-box{
        display: inline-block;
        width: 700px;
        p{
        font-size: 14px;
        color: #999;
        line-height: 22px;
        }
      }

      .sponsor-list{
        width:100%;
        padding-top: 10px;
        text-align: center;
        .table{
          display: table;
          border-collapse: collapse;
          height: 160px;
          margin: auto;
          .tr{
            display: table-row;
            height: 60px;
            .td{
              display: table-cell;
              width:180px;
              text-align: center;
              vertical-align: middle;
              table-layout: fixed;
              img{
                margin-left: 15px;
                width: 157px;
                height: 50px;
                display: block;
                border: dashed 1px #999;
              }
            }
          }
        }
      }
    }
  }
  .page-footer{
    width: 100%;
    background-color: #56575a;
    margin-top: 55px;
    padding-top: 30px;
    .page-footer-box{
      width: 70%;
      display: inline-block;
      .footer-icon-list{
        .el-popover-distance{
          margin-left: 10px;
          margin-right: 10px;
        }
        // img{
        //   width:30px;
        //   height:31px;
        //   padding-left: 10px;
        //   padding-right: 10px;
        // }
      }
      .font-14{
        font-family: Roboto;
        padding-top: 10px;
        font-size: 12px;
        color: #999;
      }
      .font-12{
        font-size: 10px;
        color: #999;
      }
    }

  }

}
</style>
