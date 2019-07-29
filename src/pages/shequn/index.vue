<template>
    <div>
        <div class="head">
        <i class="sou" @click="sousuo()"></i>
      <input class="in1"       
       type="text" placeholder="请输入感兴趣的关键字和发布者昵称"/>
      </div>
      <div>
    <div class="navbar">
      <block v-for="(item,index) in tabs" :key="index">
        <div :id="index" :class="{'navbar_item_on':activeIndex == index}" class="navbar_item" @click="tabClick">
          <div class="navbar_title">{{item.name}}</div>
        </div>
      </block>
      <div class="navbar_slider" :class="navbarSliderClass"></div>
    </div>
    <div>
      <div :hidden="activeIndex != 0">
        <div class="toop">
                <scroll-view class="header-shequ" scroll-y="true">
                    <view class="header-shequ-box" v-for="(item2, index2) in hotList" :key="index2">
                        <div >  
                           
                                      <!-- <ul>
                                        <li v-for="(item3,index3) in list" :key="index3" >
                                            {{item3}}
                                        </li>
                                      </ul> -->
                           <div class="recommend_hot_image"><img :src="item2.pic"  style="width:50px;height:50px;"/></div>
                            <div class="l">讨论 </div> 
                            <div class="r">#实习租房</div>
                        </div>
                    </view>
                </scroll-view>
              </div>
              </div>
      <div :hidden="activeIndex != 1">
         <div class="wo">
          &nbsp; <br/>
          &nbsp;&nbsp;&nbsp;&nbsp;Hello! <br/>
          &nbsp;<br/>
          &nbsp;&nbsp;&nbsp;&nbsp;您目前没有加入任何社群<br/>
          &nbsp;<br/>
          &nbsp;&nbsp;&nbsp;&nbsp;您可以<span @click="dofn()" style="color: #3185ff">所有社群</span>或<span @click="dofn()" style="color: #3185ff">搜索</span>  
          <br/>&nbsp;<br/>
          &nbsp;&nbsp;&nbsp;&nbsp;寻找并加入自己的社群<br/>&nbsp;<br/>
          &nbsp;&nbsp;&nbsp;&nbsp;也可以自己<span @click="dofn()" style="color: #3185ff">创建社群</span> 
        </div>
      </div>
    </div> 
    <!-- <swiper class="content" :duration="50" :style="'height:'+contentHeight" @change="swiperChange" :current="currentTab" @animationfinish="onAnimationfinish">
        <swiper-item  v-for="(item,index) in tabs" :key="index">
          <div class="navbar_slider_0 ">
              
      </div>
        </swiper-item>
      </swiper> -->
  </div>
  <div  class="getUserInfobutton-hover" style="height:36px;width:130px;" @click="dofn()">
        <img src="../../../static/images/establish.png" alt="" role="img" class="im"/>
  </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
          // list:[],
            hotList: [
          { 
            pic: require('../../../static/images/user.png'),
          }, {
            pic: require('../../../static/images/user.png'),
          }, {
            pic: require('../../../static/images/user.png'),
          }, {
            pic: require('../../../static/images/user.png'),
          }, {
            pic: require('../../../static/images/user.png'),
          },{
            pic: require('../../../static/images/user.png'),
          },{
            pic: require('../../../static/images/user.png'),
          },{
            pic: require('../../../static/images/user.png'),
          },
          {
            pic: require('../../../static/images/user.png'),
          }
        ],
            tabs: [
        {
          name: "所有社群",
          type: "0",
          checked: true
        },
        {
          name: "我的社群",
          type: "1",
          checked: true
        }
      ],
      activeIndex: 0,
      currentTab: 0,
      winWidth: 0,
      winHeight: 0,
        }
    },
     computed: {
    navbarSliderClass() {
      if (this.activeIndex == 0) {
        return "navbar_slider_0";
      }
      if (this.activeIndex == 1) {
        return "navbar_slider_1";
      }
    },
    contentHeight() {
      return this.winHeight + "px";
    }
  },
  methods: {
    dofn(){
      const url='../community/main'
      wx.navigateTo({url});
    },
    sousuo(){

    },
    tabClick(e) {
      this.activeIndex = e.currentTarget.id;
    },swiperChange(e) {
      this.currentTab = e.mp.detail.current;
      this.activeIndex = this.currentTab;
    },

    onAnimationfinish() {
      console.log("滑动完成.....")
    }
  },onLoad() {
    var res = wx.getSystemInfoSync();
    this.winWidth = res.windowWidth;
    this.winHeight = res.windowHeight;
  },
  // created(){
  //   for(var i=1;i<10;i++){
  //     this.list.push(i);
  //   }
  // }
}
</script>
<style>
    .head{
        width: 364px;
        margin-top: 5px;
        margin-left: 5px;
        height: 35px;
        background-color: rgba(30, 31, 31, 0.164);
        position: relative;
        border-radius: 20px;
    }
    .in1{
        margin-left:30px; 
        width: 320px;
        height: 35px;
        float: left;
        background-color:transparent;
    }
    .sou{
        background: url(../../../static/images/serch.png) ;
        margin-top:10px; 
        margin-left: 10px;
        width: 16px;
        height: 16px;
        position: absolute;
    }
    .content {
  box-sizing: border-box;
  height: 100%;
  padding-top: 50px;
  -webkit-overflow-scrolling: touch;
}

.swiper-item {
  height: 100%;
  text-align: center;
}

.navbar {
  display: -webkit-box;
  display: -webkit-flex;
  display: flex;
  position: absolute;
  z-index: 500;
  top: 40;
  height: 50px;
  width: 100%;
  background-color: white;
  border-bottom: 1rpx solid #ccc;
}

.navbar_item {
  position: relative;
  display: block;
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  flex: 1;
  padding: 13px 0;
  text-align: center;
  font-size: 0;
}

.navbar_item .navbar_item_on {
  color: white;
}

.navbar_title {
  color: #3185ff;
  font-weight: 500;
  display: inline-block;
  font-size: 15px;
  max-width: 8em;
  width: auto;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  word-wrap: normal;
}.header-shequ{
  position: absolute;
  margin-top: 50px;
  
}
.header-shequ-box{
  border-bottom: 1rpx solid #ccc;
  height: 60px;
}
.navbar_slider {
  position:absolute;
  content: " ";
  left: 0;
  bottom: 0;
  width: 6em;
  height: 2px;
  background-color:#298de5;
  -webkit-transition: -webkit-transform 0.1s;
  transition: -webkit-transform 0.1s;
  transition: transform 0.1s;
  transition: transform 0.1s, -webkit-transform 0.1s;
}

.navbar_slider_0 {
  left: 29rpx;
  transform: translateX(50rpx);
}

.navbar_slider_1 {
  left: 29rpx;
  transform: translateX(450rpx);
}
.controls {
  display: -webkit-box;
  display: -webkit-flex;
  display: flex;
  position: absolute;
  z-index: 8888;
  top: 80;
  height: 50px;
  width: 100%;
  background-color: black;
}
.recommend_scroll_x_box {
  height: 245px;
  white-space: nowrap;
  display: flex;
}
::-webkit-scrollbar { 
  width: 0;
  height: 0;
  color: transparent;
}
.recommend_hot_image{
width:50px;
height:50px;
float: left;
position:absolute;
margin-left: 40px ;
}
.l{
  position: relative;
    width: 40px;
    margin-top: 15px;
    margin-right: 40px;
    float: right;
}
.r{
  padding-top: 15px;
  margin-left: 100px;
  width: 80px;
}
.wo{
  width: 250px;
  height: 285px;
  position:absolute;
  margin-top: 100px;
  margin-left: 70px;
  background: url(../../../static/images/msg.png) ;
  background-size: 100%;
  color: #999999;
  font-size: 18px;
}
.im{
width:212rpx;
height:68rpx;
position:relative;
display:inline-block;
overflow:hidden;
}
.getUserInfobutton-hover{
position:fixed;
right:30rpx;
bottom:100rpx;
padding:0;
/* color:rgba(53, 53, 53, 0.6);
border-color:rgba(7, 6, 6, 0.6); 
 border:1px solid #353535; */
display:block;
box-sizing:border-box;
font-size:18px;
text-align:center;
text-decoration:none;
line-height:2.55555556;
-webkit-tap-highlight-color:transparent;
overflow:hidden;

}

</style>
