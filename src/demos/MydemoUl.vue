<template>
  <div class="myuldiv">
  <ul class="mydemoul">
    <li class="mydemoli" v-for="item in lidatas">
        <i :class="'icon '+ item.className"></i>
      <span v-text="item.lable"></span>
    </li>
  </ul>
  </div>
</template>
<script>
  export default {
    props: ['lidata'],
    data: function () {
      return { lidatas: this.lidata }
    }
  }
</script>
<style scoped>
  @import '~vux/src/styles/iconfont.less';

  .mydemoul{
    content: "";
    display: block;
    clear: both;
    margin: 0;
    padding: 0;
    height: 100%;
  }
  .myuldiv {
    flex: 1 auto;
    overflow: auto;
  }
  .mydemoul:after{
    content: "";
    display: block;
    clear: both;
  }
  .myuldiv{
    height: auto;
  }
  .mydemoli{
    display: block;
    float: left;
    background: white;
    width: 33.3%;
    height: 100px;
    text-align: center;
    font-size: 14px;
    font-weight: 600;
    border: 1px solid #eee;
    border-radius: 4px;
    box-sizing: border-box;
    padding: 20px;
  }
  .mydemoli .icon {
    display: inline-block;
    width: 40px;
    height: 40px;
    line-height: 40px;
    border-radius: 4px;
    color: white;
  }

  .mydemoli:last-child .icon{
    color: #aaa;
  }
  .mydemoli span:last-child{
    display: block;
    margin-top: 5px;
  }
  .i-xiaoxi:before {
    content: "\e60a";
  }
  .menubg1{
    background: #F17486;
  }
  .menubg2{
    background: #DDD25F;
  }
  .menubg3{
    background: #41B7E8;
  }
  .menubg4{
    background: #AEC2F4;
  }

</style>
