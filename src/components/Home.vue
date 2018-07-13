<template>
  <div class="Home">
    <div class="header">
      <mt-navbar v-model="selected">
        <mt-tab-item id="1">Dinning</mt-tab-item>
        <mt-tab-item id="2">Shopping</mt-tab-item>
        <mt-tab-item id="3">Lifestyle</mt-tab-item>
      </mt-navbar>
    </div>
    <!-- <a :  href=                      " ['index.html?id='+sf1] "                     > -->
    <!-- href="tel:{{item.phone}}" -->
    <!-- tab-container -->
    <mt-tab-container v-model="selected">
      <mt-tab-container-item id="1">
        <div class="container">
          <a v-for='(item,inde) in Dinning' :href="['tel:'+ item.phone]">
            <div class="item clearfix">
              <div class="item-img">
                <img :src="item.img" height="70" width="70" alt="">
              </div>
              <div class="item-info">
                <div class="name">{{item.name}}</div>
                <div class="addr">{{item.addr}}</div>
                <div class="phone"> <span class="icon"></span> {{item.phone}}</div>
              </div>
            </div>
          </a>
        </div>
      </mt-tab-container-item>
      <mt-tab-container-item id="2">
        <div class="container">
          <a v-for='(item,inde) in Shopping' :href="['tel:'+ item.phone]">
            <div class="item clearfix">
              <div class="item-img">
                <img :src="item.img" height="70" width="70" alt="">
              </div>
              <div class="item-info">
                <div class="name">{{item.name}}</div>
                <div class="addr">{{item.addr}}</div>
                <div class="phone"> <span class="icon"></span> {{item.phone}}</div>
              </div>
            </div>
          </a>
        </div>
      </mt-tab-container-item>
      <mt-tab-container-item id="3">
        <div class="container">
          <a href="tel:0147-88469258">
            <div class="item clearfix">
              <div class="item-img">
                <img src="../assets/Bitmap.png" height="70" width="70" alt="">
              </div>
              <div class="item-info">
                <div class="name">浦东鸿艺会 AMBASSY CLUB</div>
                <div class="addr">红枫路588号 588 Hongfeng</div>
                <div class="phone"> <span class="icon"></span> 021-5198 3688</div>
              </div>
            </div>
          </a>
        </div>
      </mt-tab-container-item>
    </mt-tab-container>
  </div>
</template>

<script>
var Dinning = [
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/2_cameo.png',
    name: '卡美奥意大利艺术餐厅  CAMEO RISTORANT ITALIANO',
    addr: '碧云路633号  A2，633 Biyun Rd',
    phone: '50302166'
  },
  {
    img: '/static/img/Dinning/3_bluefrog.png',
    name: '蓝蛙  BLUE FROG',
    addr: '碧云路633号 A3，633 Biyun Rd',
    phone: '50306426'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },

];
var Shopping = [
  {
    img: '/static/img/Dinning/1_STARBUCKS.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: '/static/img/Dinning/2_cameo.png',
    name: '卡美奥意大利艺术餐厅  CAMEO RISTORANT ITALIANO',
    addr: '碧云路633号  A2，633 Biyun Rd',
    phone: '50302166'
  }
]
export default {
  name: 'Home',
  data () {
    return {
     selected: "1",
     Dinning: Dinning,
     Shopping: Shopping
    }
  },
  watch: {
    selected: function () {
      document.body.scrollTop = 0;
      document.documentElement.scrollTop = 0;
    }
  }
}
</script>

<style scoped>
a {
  text-decoration: none;
}
a,img,button,input,textarea{-webkit-tap-highlight-color:rgba(255,255,255,0);}
.mint-navbar .mint-tab-item .mint-tab-item-label {
  font-size: 50px !important;
}
.clearfix:after {
   content:""; 
   display: block; 
   clear:both; 
}
.mint-tabbar{
.mint-tab-item{
  .mint-tab-item-label{
    font-size: 30px;
  }
}
}
.Home {
  padding-top: 52px;
}
.header {
  position: fixed;
  left: 0;
  top: 0;
  height: 46px;
  width: 100%;
  z-index: 100;
}
.mint-navbar {
  background-color: #295F4E;
}
.mint-navbar .mint-tab-item {
  color: #B8DED2;
  position: relative;
}
.mint-navbar .mint-tab-item .mint-tab-item-label {
  font-size: 16px !important;
}

.mint-navbar .mint-tab-item.is-selected {
  color: #fff;
  border-bottom: none;
}
.mint-navbar .mint-tab-item.is-selected:after {
  content: '.';
  position: absolute;
  width: 0;
  height: 0;
  left: 0;
  right: 0;
  top: auto;
  bottom: 3px;
  margin: auto;
  background-color: #295F4E;
  font-size: 0;
  line-height: 0;
  border-width: 6px;
  border-color: #fff;
  border-top-width: 0;
  border-style: dashed;
  border-bottom-style: solid;
  border-left-color: transparent;
  border-right-color: transparent;
}
.container {
  padding:  0 12px;
}
.item {
  padding: 12px 0;
  border-bottom: 1px solid #dfdfdf;
}
.item-img {
  float: left;
}
.item-info {
  /*float: left;*/
  padding-left: 82px;
}
.item-info .name {
  color: #222;
  font-size: 16px;
}
.item-info .addr {
  color: #222;
  font-size: 14px;
  padding: 5px 0;
}
.item-info .phone {
  color: #295F4E;
  font-size: 14px;
}
.item-img img {
  width: 70px;
  height: 70px;
  border-radius: 8px;
}
.icon {
  width: 16px;
  height: 16px;
  display: inline-block;
  background: url('../assets/phone.svg') no-repeat;
  background-size: 100% 100%;
  float: left;
  margin-right: 5px;
}
</style>
