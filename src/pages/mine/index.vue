<template>
    
    <div>
        <div class="qian-nav">
            <div class="qian-nav-left" @click="Scan_sign_in()">
                <div class="qian-nav-border">
                    <i-icon type="task" size="50" color="00B266"/>
                    <a>扫描签到</a>
                </div>
                
            </div>
            <div class="qian-nav-right" @click="sign_in()">
                <div class="qian-nav-border">
                    <i-icon type="flag" size="50" color="00B266"/>
                    <a>发起签到</a>
                </div>
            </div>
        </div>

    </div>
</template>
<script>
import card from '@/components/card'
export default {


    
    components: {
        card
    },
    "usingComponents": {
        "i-icon": "../../dist/icon/index"
    }
}
</script>
<style>
.qian-nav{
    width: 100%;
    height: 300px;
    position: relative;
    /* background-color: bisque; */

}
.qian-nav-left{
  
    margin-top: 10px;
    height: 100px;
    width: 155px;
    margin-top: 10px;
    margin-left:20px;
    position: absolute;
    text-align: center;
    border-radius: 10px;
    /* background-color: aquamarine; */
    color: rgb(201, 206, 201);
    border: 2px solid rgb(208, 214, 208); 
}
.qian-nav-left a{
    color: #666;
}
.qian-nav-right a{
    color: #666;
}
.qian-nav-border{

    margin-top: 17px;
    
    
}
.qian-nav-right{
    text-align: center;
    margin-top: 10px;
    height: 100px;
    width: 155px;
    position: absolute;
    margin-top: 10px;
    margin-left: 200px;
    border-radius: 10px;
    /* background-color: blue; */
    color: rgb(201, 206, 201);
    border: 2px solid rgb(208, 214, 208);
}
.icon-search {
  background: url(../../../static/images/serach.png) no-repeat;
  width: 20px;
  height: 20px;
  position: absolute;
  top: 5px;
  left: 40px;
}
.inp1 {
  border-radius: 50px;
  padding-left: 60px;
  background-color: #9999991e;
  width: 270px;
  height: 30px;
  margin: 0 auto;
}
</style>
