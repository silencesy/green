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
          <a v-for='(item,inde) in Lifestyle' :href="['tel:'+ item.phone]">
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
    </mt-tab-container>
  </div>
</template>

<script>
var Dinning = [
  {
    img: './static/img/Dinning/1.png',
    name: '星巴克  STARBUCKS',
    addr: '碧云路633号  A1，633 Biyun Rd',
    phone: '50303537'
  },
  {
    img: './static/img/Dinning/2.png',
    name: '卡美奥意大利艺术餐厅  CAMEO RISTORANT ITALIANO',
    addr: '碧云路633号  A2，633 Biyun Rd',
    phone: '50302166'
  },
  {
    img: './static/img/Dinning/3.png',
    name: '蓝蛙  BLUE FROG',
    addr: '碧云路633号 A3，633 Biyun Rd',
    phone: '50306426'
  },
  {
    img: './static/img/Dinning/4.png',
    name: '克比印度餐厅  KEBABS ON THE GRILL',
    addr: '碧云路633号  A4，633 Biyun Rd',
    phone: '50302005'
  },
  {
    img: './static/img/Dinning/5.png',
    name: '拉蒂娜  LITNA',
    addr: '碧云路633号  A5，633 Biyun Rd',
    phone: '50306672'
  },
  {
    img: './static/img/Dinning/6.png',
    name: '天泰  SIMPLY THAI',
    addr: '碧云路633号  A6，633 Biyun Rd',
    phone: '4000007117'
  },
  {
    img: './static/img/Dinning/7.png',
    name: '黔香阁  QIAN RESTAURANT',
    addr: '碧云路633号  B29-31，633 Biyun Rd',
    phone: '68861877'
  },
  {
    img: './static/img/Dinning/8.png',
    name: '宜芝多  ICHIDO',
    addr: '碧云路633号  B27-28，633 Biyun Rd',
    phone: '50677031'
  },
  {
    img: './static/img/Dinning/9.png',
    name: '隆日本料理  RIYO',
    addr: '碧云路633号  B25-26，633 Biyun Rd',
    phone: '50306212'
  },
  {
    img: './static/img/Dinning/10.png',
    name: '彼德西餐  PETER’S',
    addr: '碧云路633号  B23-24，633 Biyun Rd',
    phone: '58908835'
  },
  {
    img: './static/img/Dinning/11.png',
    name: '两个爸爸的寿司店  CHICHI SUSHI',
    addr: '碧云路633号   633 Biyun Rd',
    phone: '50807391'
  },
  {
    img: './static/img/Dinning/12.png',
    name: '华越楼  HUAYUE GARDEN',
    addr: '碧云路633号  B21-22，633 Biyun Rd',
    phone: '58907571'
  },
  {
    img: './static/img/Dinning/13.png',
    name: '饮琢  ENJOY BAR',
    addr: '碧云路633号  D1-C3，633 Biyun Rd',
    phone: '58378205'
  },
  {
    img: './static/img/Dinning/14.png',
    name: '飞狐  FLYING FOX',
    addr: '红枫路225号  225 Hongfeng Rd',
    phone: '50309807'
  },
  {
    img: './static/img/Dinning/15.png',
    name: '乐泰  LAS TAPAS',
    addr: '红枫路259号  259 Hongfeng Rd',
    phone: '33821686'
  },
  {
    img: './static/img/Dinning/16.png',
    name: '荷风细雨  HE’S HOUSE',
    addr: '红枫路293号  293 Hongfeng Rd',
    phone: '50898820'
  },
  {
    img: './static/img/Dinning/17.png',
    name: '新元素  ELEMENT FRESH',
    addr: '红枫路331号  331 Hongfeng Rd',
    phone: '33821700'
  },
  {
    img: './static/img/Dinning/18.png',
    name: '蓝枪鱼  BLUE MARLIN',
    addr: '红枫路357号  357 Hongfeng Rd',
    phone: '68860706'
  },
  {
    img: './static/img/Dinning/19.png',
    name: '大竹  BIG BAMBOO',
    addr: '红枫路381号  381 Hongfeng Rd',
    phone: '50301779'
  },
  {
    img: './static/img/Dinning/20.png',
    name: '咖世家咖啡  COSTA COFFEE',
    addr: '红枫路399号    399 Hongfeng Rd',
    phone: '58990226'
  },
  {
    img: './static/img/Dinning/21.png',
    name: '女枪手  PISTOLERA',
    addr: '碧云路855号  855 Biyun Rd',
    phone: '50304228'
  },
  {
    img: './static/img/Dinning/22.png',
    name: '大马可意大利餐厅  DA MARCO',
    addr: '碧云路875号  875 Biyun Rd',
    phone: '50302166'
  },
  {
    img: './static/img/Dinning/23.png',
    name: '兰日本料理  RAN',
    addr: '碧云路895号  895 Biyun Rd',
    phone: '50305681'
  },
  {
    img: './static/img/Dinning/24.png',
    name: '伊仕威仕餐厅  EAST WEST RESTAURANT',
    addr: '碧云路777号  777 Biyun Rd',
    phone: '50302653'
  },
  {
    img: './static/img/Dinning/25.png',
    name: '上海老站•东  YE OLDE STATION EAST',
    addr: '碧云路1177号  1177 Biyun Rd',
    phone: '58377377'
  },
  {
    img: './static/img/Dinning/26.png',
    name: '丰和日丽  THE FESTIVAL',
    addr: '明月路1212号  1212 Mingyue Rd',
    phone: '50551877'
  },
  {
    img: './static/img/Dinning/27.png',
    name: 'JAMAICA BLUE COFFEE',
    addr: '碧云路576号  576 Biyun Rd',
    phone: '50470357'
  },

];
var Shopping = [
  {
    img: './static/img/shopping/1.png',
    name: '泰晤士杂货商店  TIMES GROCERY',
    addr: '黄杨路115号  115 Huangyang Rd',
    phone: '58385609'
  },
  {
    img: './static/img/shopping/2.png',
    name: '城市超市  CITY SHOP',
    addr: '红枫路480号  480 Hongfeng Rd',
    phone: '58360570'
  },
  {
    img: './static/img/shopping/3.png',
    name: '迪卡侬  DECATHLON',
    addr: '蓝天路600号  600 Lantian Rd',
    phone: '50307558'
  },
  {
    img: './static/img/shopping/4.png',
    name: '三夫户外  SANFO OUTDOOR STORE',
    addr: '碧云路622号  622 Biyun Rd',
    phone: '61059299'
  },
  {
    img: './static/img/shopping/5.png',
    name: '空气净化器  BLUE AIR',
    addr: '碧云路566号  566 Biyun Rd',
    phone: '61520308'
  },
  {
    img: './static/img/shopping/0.png',
    name: 'MU GALLERY',
    addr: '碧云路590号  590 Biyun Rd',
    phone: '61945980'
  },
  {
    img: './static/img/shopping/7.png',
    name: '怡品  YIPIN PARTYS',
    addr: '碧云路633号  1D2-4，633 Biyun Rd ',
    phone: '58209908'
  },
  {
    img: './static/img/shopping/0.png',
    name: '米兰站  MILAN STATION',
    addr: '碧云路633号  C5，633 Biyun Rd ',
    phone: '50307161'
  },
  {
    img: './static/img/shopping/9.png',
    name: '伊人画廊  YINREN’S GALLERY',
    addr: '碧云路633号  B14，633 Biyun Rd',
    phone: '50309570'
  },
  {
    img: './static/img/shopping/10.png',
    name: '思安德瑞羊绒生活馆  SAND RIVER',
    addr: '碧云路633号  1D2-1，633 Biyun Rd',
    phone: '68880737'
  },
  {
    img: './static/img/shopping/0.png',
    name: '五富珑行  FIVE PHILO',
    addr: '碧云路987号  987 Biyun Rd+',
    phone: '50206529'
  },
  {
    img: './static/img/shopping/0.png',
    name: '爱婴室母婴品质生活馆  BABEMAX',
    addr: '碧云路512号  512 Biyun Rd',
    phone: '68829020'
  },
  {
    img: './static/img/shopping/0.png',
    name: 'LAO-WINES WINE DELIVERY SERVICE',
    addr: '碧云路568号  568 Biyun Rd',
    phone: '13564831948'
  },
  {
    img: './static/img/shopping/14.png',
    name: '苹果授权经销商  ISPOT',
    addr: '碧云路612号  612 Biyun Rd',
    phone: '61097545'
  },
  {
    img: './static/img/shopping/15.png',
    name: 'T-House',
    addr: '碧云路636号  636 Biyun Rd',
    phone: '50811223'
  },
  {
    img: './static/img/shopping/0.png',
    name: 'SAL’S Artique',
    addr: '碧云路554号  554 Biyun Rd',
    phone: ''
  },
  {
    img: './static/img/shopping/0.png',
    name: '碧邦孕装',
    addr: '红枫路580号  580 Hongfeng Rd',
    phone: ''
  }
];
var Lifestyle = [
  {
    img: './static/img/lifestyle/1.png',
    name: '浦东鸿艺会  AMBASSY CLUB',
    addr: '红枫路588号  588 Hongfeng Rd',
    phone: '51983688'
  },
  {
    img: './static/img/lifestyle/2.png',
    name: '功夫宝贝  KUNGFU KIDS',
    addr: '碧云路562号  562 Biyun Rd',
    phone: '61945933'
  },
  {
    img: './static/img/lifestyle/3.png',
    name: '美格菲健身中心  MEGAFIT',
    addr: '碧云路600号  600 Biyun Rd',
    phone: '50308118'
  },
  {
    img: './static/img/lifestyle/4.png',
    name: '美格菲健身中心  MEGAFIT',
    addr: '黄杨路25号  25 Huangyang Rd',
    phone: '58860199'
  },
  {
    img: './static/img/lifestyle/5.png',
    name: '悠庭保健  DRAGONFLY',
    addr: '碧云路616号    616 Biyun Rd',
    phone: '58352118'
  },
  {
    img: './static/img/lifestyle/6.png',
    name: '桑格水疗会所  SUBCONSCIOUS DAYSPA',
    addr: '碧云路633号  B17，633 Biyun Rd',
    phone: '50307382'
  },
  {
    img: './static/img/lifestyle/7.png',
    name: '丝 • 廷美体会所  ZETA VILLA',
    addr: '黄杨路25号美格菲会所3楼   3F，Megafit club,25 Huangyang Rd',
    phone: '58330186'
  },
  {
    img: './static/img/lifestyle/8.png',
    name: '浩翔美容美发  81 WEST',
    addr: '碧云路633号  B15，633 Biyun Rd',
    phone: '50306981'
  },
  {
    img: './static/img/lifestyle/9.png',
    name: '子俊美业  Y • BEAUTY',
    addr: '碧云路606号  606 Biyun Rd',
    phone: '561059288'
  },
  {
    img: './static/img/lifestyle/10.png',
    name: '维美美甲  WEIMEI NAIL SALON',
    addr: '碧云路633号  1D2-2，633 Biyun Rd',
    phone: '68411807'
  },
  {
    img: './static/img/lifestyle/11.png',
    name: '知竹社  ELITE EDUCATIONAL INSTITUTE',
    addr: '云山路1789号  1789 Yunshan Rd',
    phone: '60293805'
  },
  {
    img: './static/img/lifestyle/12.png',
    name: '蒙特梭利幼儿园  MONTESSORI ACADEMY',
    addr: '碧云路1087号D栋  D1087 Biyun Rd',
    phone: '66867727'
  },
  {
    img: './static/img/lifestyle/13.png',
    name: '爱马德汉语学校 IMANDARIN',
    addr: '云山路1779号  1779 Yunshan Rd',
    phone: '61059572'
  },
  {
    img: './static/img/lifestyle/0.png',
    name: '德清会齿科  TOKUSHINKAI DENTAL CLINIC',
    addr: '蓝桉路160号  160 Lan’an Rd',
    phone: '50307858'
  },
  {
    img: './static/img/lifestyle/0.png',
    name: '尚美齿科  PURESMILE',
    addr: '碧云路650号  650 Biyun Rd',
    phone: '61059400'
  },
  {
    img: './static/img/lifestyle/16.png',
    name: '百汇医疗  PARKWAY',
    addr: '碧云路997号  997 Biyun Rd',
    phone: '64455999'
  },
  {
    img: './static/img/lifestyle/17.png',
    name: '华氏大药房  HUASHI PHARMACY',
    addr: '碧云路633号  1D3-1，633 Biyun Rd',
    phone: ''
  },
  {
    img: './static/img/lifestyle/18.png',
    name: '米乐布提宠物生活馆  MIGNON-BOUTIQUE',
    addr: ' 碧云路646号  646 Biyun Rd',
    phone: '61099860'
  },
  {
    img: './static/img/lifestyle/19.png',
    name: '外航商旅  FASCO BUSINESS TRAVEL',
    addr: '碧云路550号  550 Biyun Rd',
    phone: '61059500'
  },
  {
    img: './static/img/lifestyle/20.png',
    name: '通济隆全球外币兑换  TRAVELEX WORLDWIDE MONEY',
    addr: '碧云路633号  1Y1-3，633 Biyun Rd',
    phone: '33821682'
  },
  {
    img: './static/img/lifestyle/21.png',
    name: '国大药房  GUODA DRUGSTORE',
    addr: '黄杨路987号  987 Huangyang Rd',
    phone: ''
  },
  {
    img: './static/img/lifestyle/22.png',
    name: '童绘视觉艺术中心  ARTSPIRE',
    addr: '碧云路1037号美2楼  2F，1037 Biyun Rd',
    phone: '4000303096'
  },
  {
    img: './static/img/lifestyle/23.png',
    name: '华隆堂  HUA LONG TANG',
    addr: '红枫路618号  618 Hongfeng Rd',
    phone: '68881620'
  },
  {
    img: './static/img/lifestyle/24.png',
    name: '汇丰银行  HSBC',
    addr: '碧云路633号  633 Biyun Rd',
    phone: '38883111'
  },
  {
    img: './static/img/lifestyle/25.png',
    name: '中国银行  BANK OF CHINA',
    addr: '云山路1767号  1767 Yunshan Rd',
    phone: '61059385'
  },
  {
    img: './static/img/lifestyle/26.png',
    name: '安信证券',
    addr: '碧云路554号  554 Biyun Rd',
    phone: '58370669'
  },
  {
    img: './static/img/lifestyle/27.png',
    name: 'ROBIN N SAND',
    addr: '碧云路568号  568 Biyun Rd',
    phone: ''
  },
  {
    img: './static/img/lifestyle/28.png',
    name: '礼韵堂',
    addr: '碧云路568号  568 Biyun Rd',
    phone: '60140677'
  }
]
export default {
  name: 'Home',
  data () {
    return {
     selected: "1",
     Dinning: Dinning,
     Shopping: Shopping,
     Lifestyle: Lifestyle
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
  line-height: 24px;
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
