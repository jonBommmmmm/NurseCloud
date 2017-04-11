<template>
  <div class="head">
    <div class="top">
      <p class="image1"><span class="iconfont icon-saozhou"></span></p>
      <p class="btn">
        <a href="#medical_people" class="on">护理员</a>
        <a href="#teachers">管理老师</a>
      </p>
      <p class="image1 image2"><span class="iconfont icon-sousuo_sousuo"></span></p>
    </div>
    <div class="condition">
      <ul class="condition_n">
        <li class="one">
          <p><span>护理类型</span><i>></i></p>
          <ul class="condition_l" style="display:none;">
            <li>周期护</li>
            <li>天天护(标准)</li>
            <li>月月护(标准)</li>
          </ul>
        </li>
        <li class="two">
          <p><span>护龄</span><i>></i></p>
          <ul class="condition_l" style="display:none;">
            <li>不限</li>
            <li>2年以下</li>
            <li>2到5年</li>
          </ul>
        </li>
        <li class="three">
          <p><span>级别</span><i>></i></p>
          <ul class="condition_l" style="display:none;">
            <li>不限</li>
            <li>初级</li>
            <li>中级</li>
          </ul>
        </li>
        <li class="four">
          <p><span>筛选</span><i>></i></p>
          <ul class="condition_l" style="display:none;">
            <li>20-29</li>
            <li>30-39</li>
            <li>40-49</li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>

</script>
<style scoped>

  @import '~vux/src/styles/iconfont.less';

  .head{
    width: 100%; border-top: 1px solid transparent; font-family: microsoft yahei;
    position: absolute; top: 0; left: 0; z-index: 1000; margin-top: -1px;
  }
  .head>.top{
    text-align: center; padding-top: 20px; background-color: #f8f9fb;
  }
  .head>.top p{
    display: inline-block;
  }
  .head>.top p.image1{
    float: left; margin: 0 16px; width: 20px; height: 20px; margin-top: 5px;
  }
  .head>.top p.image1 span{
    font-size: 22px;
  }
  .head>.top p.btn{
    width: 150px; height: 30px; border: 1px solid #33bd9b; border-radius: 4px; font-size: 0; line-height: 30px;
  }
  .head>.top p.btn a{
    display: inline-block; width: 50%; height: 100%; border: 0; outline: 0; background-color: #fff; font-size: 14px; color: #33bd9b;
    border-top-right-radius: 4px; border-bottom-right-radius: 4px; cursor: pointer;
  }
  .head>.top p.btn .on{
    background-color: #33bd9b; color: #fff; border-top-right-radius: 0; border-bottom-right-radius: 0;
  }
  .head>.top p.image2{
    float: right;
  }
  .head .condition {
    background-color: #f8f9fb; border-top: 1px solid transparent;
  }
  .head .condition .condition_n{
    height: 36px; font-size: 0; margin-top: 10px; border-bottom: 1px solid #ddd; position: relative;
  }
  .head .condition .condition_n>li{
    width: 100%; position: absolute; top: 0; left: 0; box-sizing:border-box;
  }
  .head .condition .two{
    margin-left: 25%; z-index: 1;
  }
  .head .condition .three{
    margin-left: 50%; z-index: 2;
  }
  .head .condition .four{
    margin-left: 75%; z-index: 3;
  }
  .head .condition .two .condition_l{
    margin-left: -25%;
  }
  .head .condition .three .condition_l{
    margin-left: -50%;
  }
  .head .condition .four .condition_l{
    margin-left: -75%;
  }
  .head .condition .condition_n>li>p{
    display: inline-block; font-size: 16px; width: 25%; text-align: center; color: #535554; border-right: 1px solid #e9e9e9;
    margin: 10px 0; box-sizing:border-box;
  }
  .head .condition .condition_l li{
    width: 100%; height: 36px; line-height: 36px; border-bottom: 1px solid #ddd; color: #5d5d5d; font-size: 15px;
    padding-left: 14px; background-color: #fff; box-sizing:border-box;
  }

</style>
