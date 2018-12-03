<template>
  <div class="index">
     <!--头部-->
    <div class="header">
      <div class="header-content">
        <span>LOGO</span>
        <div class="header-right-icon"></div>
        <div class="header-right">
          <div v-for="(item, index) in navArr" :key="index">
            {{item}}
          </div>
        </div>
      </div>
    </div>
     <!--banner-->
    <div class="banner">
      <img src="../assets/banner.png"/>
    </div>
    <!--内容-->
    <div class="content">
      <div class="type">
        <div class="type-item" v-for="item in arr" :key="item">
          <img src="../assets/type1.png"/>
          <p class="type-item-text">111</p>
          <p class="type-item-desc">111</p>
        </div>
      </div>
      <div class="product">
        <p class="item-title">PRODUCT.</p>
        <p class="item-title-sub">产品中心</p>
        <div>
          <div class="product-type-right-wrap">
            <span :class="`product-type ${typeChooseIndex === index? 'active' : ''}`" v-for="(item, index) in productTypeArr" :key="index" @click="handleClickProType(index)">
              {{item}}
            </span>
          </div>
        </div>
        <div class="product-imgs">
          <div class="product-img-item">
            <img  src="../assets/demo1.png"/>
          </div>
          <div class="product-img-item">
            <img src="../assets/demo2.png"/>
          </div>
          <div class="product-img-item">
            <img src="../assets/demo5.png"/>
          </div>
          <div class='product-img-item'>
            <img src="../assets/demo4.png"/>
          </div>
          <div class="product-img-item">
            <img src="../assets/demo3.png"/>
          </div>
        </div>
        <div class="more-product"><span>更多</span><img src="../assets/more.png"/></div>
      </div>
    </div>
    <div class="about-us">
      <div class="about-us-bg">  
      </div>
      <div class="about-us-detail-wrap">
        <div class="about-us-detail">
          <img src="../assets/aboutusDetail.png"/>
          <div>
            <p>宝鸡市美诺装饰有限公司简介，由木纹砖领军品牌创始人所创立，团队拥有超过10年木纹砖品类运营经验，从研发生产、产品销售、经销提升、品牌维管等多方面引领行业发展。匠心的产品研发团队坚持每一片产品都使用优质原料，每一道工序坚持以最高标准执行；原产地坯料、意大利卡罗比亚釉料、常规墨水及各种工艺墨水......</p>
            <span class="about-us-more">MORE</span>
          </div>
        </div>
      </div>
    </div>

    <!--案例-->
    <div class="case">
      <!-- <div class="case-row"> -->
        <div class="case-col-2">
          <p class="case-title">CASE.</p>
          <p class="case-title-sub">经典案例</p>
        </div>
        <div><img src="../assets/row-1-3.png"/></div>
        <div class="case-item case-item-yellow">
          <p class="case-item-title">经典案例</p>
          <p class="case-item-desc">案例简介案例简介案例简介案例简介案例简介案例简介案例简介…</p>
        </div>
      <!-- </div>
      <div class="case-row"> -->
        <div class="case-col-2">
          <img src="../assets/row-2-1.png"/>
        </div>
        <div class="case-item">
          <p class="case-item-title">经典案例</p>
          <p class="case-item-desc">案例简介案例简介案例简介案例简介案例简介案例简介案例简介…</p>
        </div>
        <div>
         <img src="../assets/row-2-3.png"/>
        </div>
      <!-- </div>
      <div class="case-row"> -->
        <div class="case-item">
          <p class="case-item-title">经典案例</p>
          <p class="case-item-desc">案例简介案例简介案例简介案例简介案例简介案例简介案例简介…</p>
        </div>
        <div>
          <img src="../assets/row-3-2.png"/>
        </div>
        <div>
          <img src="../assets/row-3-3.png"/>
        </div>
        <div class="case-item">
          <p class="case-item-title">经典案例</p>
          <p class="case-item-desc">案例简介案例简介案例简介案例简介案例简介案例简介案例简介…</p>
        </div>
      <!-- </div>   -->
    </div>
    <div class="more-product"><span>更多</span><img src="../assets/more.png"/></div>

    <!--团队-->
    <div class="group">
      <p class="item-title">TEAM.</p>
      <p class="item-title-sub">团队</p>

      <div class="team-group">
        <div class="team-group-item">
          <img src="../assets/group1.png" class="first-img"/>
          <div class="group-item-detail">
            <p class="group-item-name">设计师姓名</p>
            <p class="group-item-title">室内设计师</p>
            <!-- <p class="group-item-desc">室内设计师室内设计师室内设计师</p> -->
          </div>
        </div>
        <div class="team-group-item team-group-item-reverse">
          <div class="group-item-detail">
            <p class="group-item-name">设计师姓名</p>
            <p class="group-item-title">室内设计师</p>
            <!-- <p class="group-item-desc">室内设计师室内设计师室内设计师</p> -->
          </div>
          <img src="../assets/group2.png"/>
        </div>
        <div class="team-group-item">
          <img src="../assets/group3.png"/>
          <div class="group-item-detail">
            <p class="group-item-name">设计师姓名</p>
            <p class="group-item-title">室内设计师</p>
            <!-- <p class="group-item-desc">室内设计师室内设计师室内设计师</p> -->
          </div>
        </div>
        <div class="team-group-item team-group-item-reverse">
          <div class="group-item-detail">
            <p class="group-item-name">设计师姓名</p>
            <p class="group-item-title">室内设计师</p>
            <!-- <p class="group-item-desc">室内设计师室内设计师室内设计师</p> -->
          </div>
          <img src="../assets/group4.png"/>   
        </div>
      </div>

      <!-- 新闻资讯 -->
      <div>
        <p class="item-title">NEWS.</p>
        <p class="item-title-sub">新闻资讯</p>

        <div class="news">
          <div class="news-item">
            <div class="news-date">
              <div class="align-center">04-12</div>
              <div class="align-right">2018</div>
            </div>
            <div>
              <p class="news-title">只知道佛山陶博会？从广交会上看陶瓷产业…</p>
              <p class="news-content">创办于1957年的广交会作为中国外贸第一促进平台，是中国外贸的晴雨表和风向标，无论是对广交会上的木纹砖厂家还是其他企业来说…</p>
            </div>
          </div>
          <div class="news-item news-center">
            <div class="news-date">
              <div class="align-center">04-12</div>
              <div class="align-right">2018</div>
            </div>
            <div>
              <p class="news-title">只知道佛山陶博会？从广交会上看陶瓷产业…</p>
              <p class="news-content">创办于1957年的广交会作为中国外贸第一促进平台，是中国外贸的晴雨表和风向标，无论是对广交会上的木纹砖厂家还是其他企业来说…</p>
            </div>
          </div>
          <div class="news-item">
            <div class="news-date">
              <div class="align-center">04-12</div>
              <div class="align-right">2018</div>
            </div>
            <div>
              <p class="news-title">只知道佛山陶博会？从广交会上看陶瓷产业…</p>
              <p class="news-content">创办于1957年的广交会作为中国外贸第一促进平台，是中国外贸的晴雨表和风向标，无论是对广交会上的木纹砖厂家还是其他企业来说…</p>
            </div>
          </div>
        </div>
        <div class="more-product"><span>更多</span><img src="../assets/more.png"/></div>
      </div>
    </div>

    <!--footer-->
    <div class="footer">
      <div class="footer-container">
        <div>
          <p>联系我们</p>
          <p>Contact us</p>
        </div>
        <div>
          <p>XXXX装修公司</p>
          <p>地址：圣诞节反馈哈是对方拉黑分段函数</p>
          <p>电话：020-86232323</p>
          <p>传真：0899-12212323</p>
        </div>
        <div>
          <p>邮箱：12312312312@163.com</p>
          <p>手机：12121231231</p>
          <p>邮箱：1231233131321</p>
        </div>
        <div>
          <div class="qr-code">二维码</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      arr: [1, 2, 3, 4, 5],
      navArr: ['首页', '关于', '产品', '案例', '团队', '新闻咨询', '联系我们'],
      typeChooseIndex: 0,
      productTypeArr: ['产品','产品3', '产品1', '产品1', '产品1']
    }
  },
  methods: {
    handleClickProType (index) {
      this.typeChooseIndex = index
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .header{
    position: fixed;
    top: 0;
    width: 100%;
    height: 93px;
    background-color: rgba(248, 243, 236, .8);
  }
  .header-content{
    width: 1200px;
    margin: 0 auto;
  }
  .header-right{
    float: right;
  }
  .header-right-icon{
    display: none;
  }
  .header-right div, .header-content span{
    display: inline-block;
    font-size: 15px;
    padding: 0 30px;
    cursor: pointer;
    line-height: 93px;
  }
  .banner img{
    width: 100%;
    height: 918px;
  }

  /*banner下面的类型*/
  .content{
    position: relative;
    width: 1200px;
    margin: 0 auto;
  }
  .content .type{
    display: flex;
    justify-content: center;
    text-align: center;
    padding: 30px 40px;
    margin-top: -81px;
    background-color: #ffffff;
    box-shadow: 0px 0px 20px 0px 
      rgba(6, 0, 1, 0.2);
  }
  .type-item{
    flex: 1;
    justify-content: center;
  }
  .type-item-text{
    font-size: 16px;
    line-height: .6em;
color:#000;
  }
  .type-item-desc{
    font-size: 12px;
    line-height: .6em;
    color: #808080;
  }
  .product{
    margin-top: 114px;
   }
  .product-title{
    font-size: 47px;
    color: #000;
  }
  .product-title::first-letter{
    border-bottom: 2px solid #000;
  }
  .product-type-right-wrap{
    float: right;
  }
  .product-type{
    display: inline-block;
    margin: 0 20px;
    opacity: 0.6;
    padding-bottom: 5px;
    text-align: center;
    border-bottom: 2px solid transparent;
    cursor: pointer;
  }
  .active{
    border-bottom:  2px solid #ffbc20;
  }
  .product-imgs {
    margin-top: 78px;
    column-count:3;
    column-gap: 10px;
  }
  .product-img-item { 
    -moz-page-break-inside: avoid;
    -webkit-column-break-inside: avoid;
    break-inside: avoid;
  }
  .product-img-item img{
    width: 100%;
  }
  .more-product{
    width: 137px;
    height: 38px;
    margin: 62px auto 0;
    border: solid 1px #000000;
    border-radius: 19px;
    text-align: center;
    line-height: 38px;
    font-size: 14px;
  }
  .more-product span, .more-product img{
    display: inline-block;
    vertical-align: middle;
  }
  .more-product img{
    margin-left: 13px;
  }

  .about-us-bg{
    width: 100%;
    height: 473px;
    margin-top: 80px;
    background: #ffbc20 url(../assets/about-us-bg.png) no-repeat center;
    background-size: 100%;
    background-clip: content-box;
  }
  .about-us-detail-wrap{
    width: 1100px;
    margin: -500px auto 0;
    padding: 51px 48px 50px 51px;
  }
  .about-us-detail{
    padding: 51px;
    background-color: #fff;
    margin-top: 306px;
    display: flex;
    flex-wrap: wrap;
  }
  .about-us-detail div{
    flex: 2;
  }
  .about-us-detail img{
    flex: 1;
    margin-right: 43px;
  }
  .about-us-detail p{
    text-indent: 20px;
    color: #686868;
    font-size: 14px;
    line-height: 37px;
  }
  .about-us-more{
    padding: 3px 30px;
    background-color: #ffbc20;
    border-radius: 19px;
    color: #fff;
  }


  /* 案例样式 */
  .case{
    width: 1200px;
    margin: 257px auto 0;
    display: flex;
    flex-wrap: wrap;
  }
  .case div{
    flex-basis: 300px;
    flex-grow: 1;
    flex-shrink: 1;
    height: 296px;
  }
  .case div img{
    width: 100%;
    height: 100%;
  }
  .case-col-2{
    flex-basis: 600px !important;
    flex-grow: 2  !important;
    flex-shrink: 2  !important;
  }
  .case-title,.item-title{
    font-size: 53px;
    color: #000;
    opacity: .8;
    margin-block-start: .5em;
    margin-block-end: .5em;
  }
  .case-title::first-letter, .item-title::first-letter{
    border-bottom: 2px solid #000;
  }
  .case-title-sub,.item-title-sub{
    font-size: 24px;
    text-indent: 9px;
    color: #5b5b5b;
  }
  .case-item{
    background-color: #fcf9f2;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .case-item-yellow{
    background-color: #ffbc20;
  }
  .case-item-title{
    font-size: 20px;
    line-height: 30px;
  }
  .case-item-desc{
    padding: 0 38px;
  }

  /* 团队 */
  .group{
    width: 1200px;
    margin: 0 auto;
  }
  .team-group{
    display: flex;
    flex-wrap: wrap;
  }
  .team-group-item{
    flex-basis: 300px;
    flex-grow: 1;
    flex-shrink: 1;
    height: 400px;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
  }
  .team-group-item img{
    width: 100%;
  }
  .group-item-detail{
    font-size: 18px;
    padding: 0 23px 0;
  }
  .group-item-detail p{
    margin-block-start: .3em;
    margin-block-end: .3em;
  }
  /*news*/
  .news{
    display: flex;
    flex-wrap: wrap;
  }
  .news-item{
    margin-right: 26px;
    flex: 1;
    flex-basis: 300px;
  }
  .news-date{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 87px;
    height: 92px;
    color: #fff;
    background-color: #2d2d2d;
  }
  .align-right{
    text-align: right;
    opacity: 0.5;
  }
  .news-title{
    font-size: 16px;
    color: #2d2d2d;
  }
  .news-item .news-content{
    font-size: 14px;
    line-height: 29px;
    color: #2d2d2d;
    opacity: 0.5;
  }
  .news-center{
    background-color: #2d2d2d;
    padding: 0 36px 58px;
    box-sizing: border-box;
  }
  .news-center .news-title, .news-center .news-content{
    color: #fff;
  }
  .news-center .news-date{
    margin-top: -16px;
    background-color: #ffbc20;
    color: #000000;
  }

  /*footer*/
  .footer{
    margin-top: 57px;
    background-color: #2d2d2d;
    color: rgba(255,255,255, .5);
  }
  .footer-container{
    padding: 60px 55px;
    width: 1200px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    font-size: 16px;
  }
  .footer div{
    flex-grow: 1;
    flex-shrink: 1;
  }
  .qr-code{
    width: 168px;
    height: 168px;
    background-color: #ffffff;
  }
  @media screen and (max-width: 1200px) {
    /*移动端兼容*/
    .index{
      width: 100vw;
      overflow: hidden;
    }
    .banner{
      margin-top: 70px;
    }
    .banner img{
      height: 40vh;
    }
    .content, .case, .about-us-detail-wrap, .group, .news, .footer-container{
      width: 90vw;
      margin: 0 auto;
    }
    .type{
      flex-wrap: wrap;
      justify-content: flex-start !important;
    }
    .type-item {
      flex-basis: 5.3rem;
      flex-grow: 0;
    }
    .header-right{
      display: none;
    }
    .header, .header-content{
      width: 100vw;
    }
    .header-right-icon{
      display: block;
      position: absolute;
      right: 0;
      top: 50%;
      transform: translate(-50%, -50%);
      padding: 6px 0;
      border-top: 3px solid;
      border-bottom: 3px solid ;
      height: 3px;
      width: 25px;
      background: #808080;
      color: #808080;
      background-clip: content-box;
    }

    .product{
      margin-top: 3rem;
    }
    .product-type-right-wrap{
      float: none;
      margin-top: 1em;
    }
    .product-type {
      margin-left: 0;
    }
    .product-imgs{
      margin-top: 1em;
      column-count: 1;
    }

    .about-us-bg{
      height: 17rem;
      padding: 0;
    }
    .about-us-detail-wrap{
      padding: 1rem;
      margin-top: -9rem;
    }
    .about-us-detail{
      padding: 1rem;
      margin-top: 0;
    }
    .about-us-detail img{
      width: 100%;
    }
    .team-group-item{
      height: auto;
    }
    .team-group-item-reverse {
      flex-direction: column-reverse;
    }
   .news-item{
     padding-bottom: 2rem;
   }
   .news-center{
     background: #fff;
     padding: 0;
   }
   .news-center .news-title, .news-center .news-content{
     color: #000;
   }
   .news-center .news-date{
     color: #fff;
     background-color: #2d2d2d;
   }


   .footer div{
     flex-basis: 12rem;
   }
  }
  
</style>
