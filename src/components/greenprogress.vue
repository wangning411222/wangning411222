<template>
  <div class="lin-box">
    <span class="max">
      <span class="num" :style="{width:num*100+'%','background':num===1?'rgb(228, 188, 49)':'#50B264'}"></span>
    </span>
    <span class="num-text" >{{num*100}}%</span>
  </div>
</template>
<script>
export default {
  props: {
    num: {
      type: Number,
      default: 0

    }
  }
}
</script>
<style lang="scss" scoped>
.lin-box{
  text-align:left;
}
.max {
  margin-right: 17px;
  width: 144px;
  height: 18px;
  position: relative;
  display: inline-block;
  background: #F2F3F4;
  border-radius:8px;
  .num {
    position: absolute;
    top:0;
    left:0;
    height: 100%;
    width: 90%;
    display: inline-block;
    border-radius:8px;
  }
  .num-text{
    color: #999999;
    font-size:20px;
  }
}
</style>
