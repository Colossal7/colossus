<template>
  <div>
      <i class="icon-search"></i>
      <input
        type="text"
        v-model="msg"
        placeholder="输入感兴趣的关键词或发布者昵称"
        placeholder-style="color: #858585;"
        class="inp1"
      />
    </div>
</template>

<script>
export default {

}
</script>

<style>

.icon-search {
  background: url(../../../static/images/serach.png) ;
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