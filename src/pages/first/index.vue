<template>
  <div>
    <div class="section">
      <i class="icon-search"></i>
      <input
        class="input-radius"
        bindinput="bindKeyInput"
        placeholder-class="center"
        placeholder="输入感兴趣的关键词或发布者"
      />
    </div>
    <div class="nav">
      <div class="left-title">职前公社</div>
      <div class="right-title" @click="jump()">
        <img src="../../../static/images/more.png" style="width:12px;height:12px" alt /> 更多
      </div>
    </div>
    <scroll-view scroll-x="true" style="height:60px; display: flex; white-space: nowrap;">
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/more.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>南巷</span>
          </div>
        </div>
      </view>
      <view style="display: inline-block; width:50px;hight:60px">
        <div class="user">
          <div class="user-top">
            <img class="head-portrait" src="../../../static/images/uploading.png" alt />
          </div>
          <div style="height:10px;font-size:10px">
            <span>上传</span>
          </div>
        </div>
      </view>
    </scroll-view>
    <div style="background-color: #f1f1f1;height:10px;width:100%;"></div>
    <div class="navbar">
      <block v-for="(item,index) in tabs" :key="index">
        <div
          :id="index"
          :class="{'navbar_item_on':activeIndex == index}"
          class="navbar_item"
          @click="tabClick"
        >
          <div class="navbar_title1" >
            <div class="navbar_title">{{item.name}}</div>
          </div>
        </div>
      </block>
      <div class="navbar_slider" :class="navbarSliderClass"></div>
    </div>
    <div :hidden="activeIndex != 0">

    <swiper
      class="content"
      :duration="50"
      :style="'height:'+contentHeight"
      @change="swiperChange"
      :current="currentTab"
      @animationfinish="onAnimationfinish"
    >
      <swiper-item v-for="(item,index) in tabs" :key="index">
        <div :key="1">
          <!-- {{item.name}} -->
          <i-cell-group>
            <div class="z-list">
              <div class="z-list-top">
                <div class="z-list-top-left">
                  <img style=" height:40px;width:40px;" src="../../../static/images/user.png" alt />
                </div>
                <div class="z-list-top-mid">
                  <!-- <i-cell  title="八岁" label="来日可期" value="bbbb"></i-cell> -->
                  <div class="z-list-top-mid-top">
                    <div class="z-list-top-mid-top-left">
                      <span>Colossus</span>
                    </div>
                    <div class="z-list-top-mid-top-right">
                      <span>1小时前</span>
                    </div>
                  </div>
                  <div class="z-list-top-mid-bottom">天津软件技术学院·网易·产品运营</div>
                </div>
              </div>
              <div class="z-list-span">
                <span>我们皆是赶路的众生，泪笑掺杂，悲喜交织，没有谁的欢乐可以长久，执手再紧亦将曲终人散。人生原本一场罪，痛苦的人，不过是自得其所；幸福的人，也只是苦中作乐。只有真切的哭过，绝望的累过，钻心的痛过，无言的悔过，此生方算完整。</span>
              </div>
              <div class="z-list-bottom">
                <div class="z-list-bottom-left">#南巷寻猫喵</div>
                <div class="z-list-bottom-right">
                  <i-icon type="like_fill" />777
                  <i-icon type="emoji_fill" />99+
                </div>
              </div>
              <div class="z-list-boder"></div>
            </div>
            <div class="z-list">
              <div class="z-list-top">
                <div class="z-list-top-left">
                  <img style=" height:40px;width:40px;" src="../../../static/images/user.png" alt />
                </div>
                <div class="z-list-top-mid">
                  <!-- <i-cell  title="八岁" label="来日可期" value="bbbb"></i-cell> -->
                  <div class="z-list-top-mid-top">
                    <div class="z-list-top-mid-top-left">
                      <span>Colossus</span>
                    </div>
                    <div class="z-list-top-mid-top-right">
                      <span>1小时前</span>
                    </div>
                  </div>
                  <div class="z-list-top-mid-bottom">天津软件技术学院·网易·产品运营</div>
                </div>
              </div>
              <div class="z-list-span">
                <span>我们皆是赶路的众生，泪笑掺杂，悲喜交织，没有谁的欢乐可以长久，执手再紧亦将曲终人散。人生原本一场罪，痛苦的人，不过是自得其所；幸福的人，也只是苦中作乐。只有真切的哭过，绝望的累过，钻心的痛过，无言的悔过，此生方算完整。</span>
              </div>
              <div class="z-list-bottom">
                <div class="z-list-bottom-left">#南巷寻猫喵</div>
                <div class="z-list-bottom-right">
                  <i-icon type="like_fill" />777
                  <i-icon type="emoji_fill" />99+
                </div>
              </div>
              <div class="z-list-boder"></div>
            </div>

            <div class="z-list">
              <div class="z-list-top">
                <div class="z-list-top-left">
                  <img style=" height:40px;width:40px;" src="../../../static/images/user.png" alt />
                </div>
                <div class="z-list-top-mid">
                  <!-- <i-cell  title="八岁" label="来日可期" value="bbbb"></i-cell> -->
                  <div class="z-list-top-mid-top">
                    <div class="z-list-top-mid-top-left">
                      <span>Colossus</span>
                    </div>
                    <div class="z-list-top-mid-top-right">
                      <span>1小时前</span>
                    </div>
                  </div>
                  <div class="z-list-top-mid-bottom">天津软件技术学院·网易·产品运营</div>
                </div>
              </div>
              <div class="z-list-span">
                <span>我们皆是赶路的众生，泪笑掺杂，悲喜交织，没有谁的欢乐可以长久，执手再紧亦将曲终人散。人生原本一场罪，痛苦的人，不过是自得其所；幸福的人，也只是苦中作乐。只有真切的哭过，绝望的累过，钻心的痛过，无言的悔过，此生方算完整。</span>
              </div>
              <div class="z-list-bottom">
                <div class="z-list-bottom-left">#南巷寻猫喵</div>
                <div class="z-list-bottom-right">
                  <i-icon type="like_fill" />777
                  <i-icon type="emoji_fill" />99+
                </div>
              </div>
              <div class="z-list-boder"></div>
            </div>
          </i-cell-group>
        </div>
      </swiper-item>
    </swiper></div>
    <div :hidden="activeIndex != 1">
    <swiper
      class="content"
      :duration="50"
      :style="'height:'+contentHeight"
      @change="swiperChange"
      :current="currentTab"
      @animationfinish="onAnimationfinish"
    >
      <swiper-item v-for="(item,index) in tabs" :key="index">
        <div>
          {{item.name}}
        </div>
      </swiper-item>
    </swiper></div>
    <div :hidden="activeIndex != 1">
    <swiper
      class="content"
      :duration="50"
      :style="'height:'+contentHeight"
      @change="swiperChange"
      :current="currentTab"
      @animationfinish="onAnimationfinish"
    >
      <swiper-item v-for="(item,index) in tabs" :key="index">
        <div>
          {{item.name}}
        </div>
      </swiper-item>
    </swiper></div>
    <div class="toolBar">
      <i-icon type="brush_fill"/>
      <span>想说</span>
    </div>
  </div>
</template>
<script>
export default {
  
  data() {
    return {
      tabs: [
        {
          name: "推荐",
          type: "1",
          checked: true
        },
        {
          name: "精选",
          type: "2",
          checked: true
        },
        {
          name: "简历",
          type: "3",
          checked: true
        }
      ],
      activeIndex: 0,
      currentTab: 0,
      winWidth: 0,
      winHeight: 0
    };
  },

  computed: {
    navbarSliderClass() {
      if (this.activeIndex == 0) {
        return "navbar_slider_0";
      }
      if (this.activeIndex == 1) {
        return "navbar_slider_1";
      }
      if (this.activeIndex == 2) {
        return "navbar_slider_2";
      }
    },
    contentHeight() {
      return this.winHeight + "px";
    }
  },
  
  methods: {
    tabClick(e) {
      this.activeIndex = e.currentTarget.id;
      this.currentTab = this.activeIndex;
    },
    swiperChange(e) {
      this.currentTab = e.mp.detail.current;
      this.activeIndex = this.currentTab;
    },
    onAnimationfinish() {
      console.log("滑动完成.....");
    },
    jump(){
      const url ='../shequn/main'
      wx.navigateTo({url})
      
    }
  },
  onLoad() {
    var res = wx.getSystemInfoSync();
    this.winWidth = res.windowWidth;
    this.winHeight = res.windowHeight;
  }
};
</script>



<style>
.nav {
  height: 40px;
  min-height: 40px;
  margin-top: 10px;
}
.left-title {
  padding-left: 10px;
  font-size: 14px;
  font-style: inherit;
  float: left;
  position: absolute;
}
.right-title {
  float: right;
  padding-right: 20px;
  font-size: 12px;
  color: #298de5;
}
.input-radius {
  background: rgb(238, 236, 236);
  border-radius: 15px;
  margin: 10px 0 3px 3px;
  width: 360px;
  height: 0.5rem;
  min-height: 0.5rem;
  font-size: 15px;
  text-align: center;
  font-size: 14px;
}
.user {
  width: 50px;
  text-align: center;
}
.head-portrait {
  width: 35px;
  height: 35px;
}
.swiper-item {
  height: 100%;
  text-align: center;
}
.navbar {
  display: -webkit-box;
  display: -webkit-flex;
  display: flex;

  /* position: absolute;
  z-index: 500;
  top: 145px;
  height: 50px;
  width: 100%; */
  background-color: #ffffff;
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
  width:0;
}

.navbar_item.navbar_item_on {
  color: #3185ff;
  border-bottom: 2px solid #3185ff;
  /* border-bottom-width:1px; */
}
.navbar_item_on .navbar_title {
  color: #3185ff;
}
/* .navbar_title1{
  width: 50px;
  height: 48px;
  border-bottom:2px solid #3185ff ;
  margin: 0 auto
} */
.navbar_title {
  color: rgb(12, 12, 12);
  font-weight: 500;
  display: inline-block;
  font-size: 15px;
  max-width: 8em;
  width: auto;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  word-wrap: normal;
}
.navbar_slider {
  position: absolute;
  content: " ";
  left: 0;
  bottom: 0;
  width: 6em;
  height: 3px;
  background-color: white;
  -webkit-transition: -webkit-transform 0.1s;
  transition: -webkit-transform 0.1s;
  transition: transform 0.1s;
  transition: transform 0.1s, -webkit-transform 0.1s;
}

.navbar_slider_0 {
  left: 29rpx;
  transform: translateX(0);
}

.navbar_slider_1 {
  left: 29rpx;
  transform: translateX(250rpx);
}

.navbar_slider_2 {
  left: 29rpx;
  transform: translateX(500rpx);
}
.controls {
  display: -webkit-box;
  display: -webkit-flex;
  display: flex;
  position: fixed;
  z-index: 8888;
  top: 80;
  height: 50px;
  width: 100%;
  background-color: #298de5;
  border-top: 2px solid rgb(103, 103, 104);
}
.z-list {
  height: 150px;
  width: 100%;

  /* background-color: #298de5; */
}
.z-list-top {
  height: 65px;
  width: 100%;
  /* border: 1px solid red; */
  position: relative;
  /* background-color: #ccc; */
}
.z-list-top-left {
  position: absolute;
  padding-left: 10px;
  padding-top: 15px;

  float: left;
  overflow: hidden;
}
.z-list-top-mid {
  width: 100%;
  height: 65px;
  float: inherit;

  /* background-color: aqua;  */
}
.z-list-top-mid-top {
  height: 30px;
  width: 100%;
  /* border: 1px solid red; */
  position: absolute;
  /* background-color: aliceblue */
}
.z-list-top-mid-top-left {
  padding-top: 15px;
  margin-left: 55px;
  float: left;
  height: 15px;
  width: 60.008%;
  /* background-color: bisque; */
  font-size: 12px;
  color: rgba(66, 66, 66, 0.836);
}
.z-list-top-mid-top-right {
  font-size: 10px;
  padding-top: 15px;
  float: right;
  height: 15px;
  width: 20%;
  color: #ccc;
}
.z-list-top-mid-bottom {
  height: 15px;
  widows: 200px;
  padding-top: 35px;
  padding-left: 55px;
  color: #ccc;
  font-size: 10px;
  /* background-color: #298de5; */
}
.z-list-span {
  font-size: 12px;
  padding-left: 15px;
  padding-right: 15px;
}
.z-list-bottom {
  /* background-color: antiquewhite; */
  height: 30px;
}
.z-list-bottom-left {
  padding-top: 7px;
  padding-left: 15px;
  width: 60%;
  font-size: 12px;
  color: #298de5;
  float: left;
  /* background-color: bisque */
}
.z-list-bottom-right {
  padding-top: 5px;
  width: 25%;
  float: right;
  font-size: 12px;
  color: #666;
}
.z-list-boder {
  background-color: #ccc;
  height: 0.1px;
}
.toolBar {
  position: fixed;

  left: 75%;
  bottom: 15%;
  width: 68px;
  height: 22px;
  color: #ffffff;
  /* border: 1px solid red; */
  border-radius: 15px;
  background-image: url(../../../static/images/x.png);
  background-repeat: no-repeat;
  background-position: center center;
  text-align: center;
  padding-top: 1px;
  font-size: 14px;
}
</style>
