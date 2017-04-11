<template>
  <div id="mydemo">
    <div class="header">
  <blur :blur-amount=40 :url="url" :height=155>
    <p class="center"><img :src="url"></p>
    <p class="content"><span v-text="name"></span></p>
  </blur>
  <flexbox :gutter=2>
    <flexbox-item>
      <div class="flex-demo">
        <span class="colorAcount1">0</span>
        <span>余额</span>
      </div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">
        <span class="colorAcount2">0</span>
        <span>积分</span>
      </div>
    </flexbox-item>
    <flexbox-item>
      <div class="flex-demo">
        <span class="colorAcount3">0</span>
        <span>优惠券</span>
      </div>
    </flexbox-item>
  </flexbox>
    </div>
   <div style="width: 100%; height: 10px;  background:#eee;"></div>
    <div class="main">
    <demoUl :lidata="demouldata"></demoUl>
    </div>
  </div>
</template>
<script>

  import { Blur, Flexbox, FlexboxItem, Grid, GridItem } from 'vux'

  import demoUl from './MydemoUl.vue'

  export default {
    components: {
      Blur,
      Flexbox,
      FlexboxItem,
      Grid,
      GridItem,
      demoUl
    },
    data () {
      return {
        url: 'https://o3e85j0cv.qnssl.com/waterway-107810__340.jpg',
        name: '未登录',
        demouldata: [{ className: 'i-aixin menubg1', lable: '收藏' }, { className: 'i-place menubg2', lable: '地址' }, { className: 'i-xiaoxi menubg3', lable: '消息中心' }, { className: 'i-wenti menubg4', lable: '常见问题' }, { className: 'i-shenglvehao', lable: '更多' }]
      }
    }
  }
</script>
<style scoped lang="less">
  @import '~vux/src/styles/1px.less';

  #mydemo{
    height: 100%;
    display: flex;
    flex-direction: column;
  }
  .menubg1 {
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
  .vux-flex-row
  {
    background:#eee;
  }
  .flex-demo {
    text-align: center;
    color: #aaa;
    background-color: white;
    border-radius: 4px;
    background-clip: padding-box;
    height:  45px;
  }
  .center {
    text-align: center;
    padding-top: 35px;
    color: #fff;
    font-size: 18px;
  }
  .center img {
    width:65px;
    height: 65px;
    border-radius: 50%;
    border: 2px solid #ececec;
  }
  .content {
    text-align: center;
    color: #fff;
    font-size: 16px;
  }
  .content span{
    width:65px;
    height: 20px;
  }
  .flex-demo span{
    line-height: 20px;
    display: block;
    font-size: 14px;
  }
  .flex-demo  span:last-child{
    display: block;
    margin-top: 5px;
  }
  .flex-demo:last-child .icon{
    color: #aaa;
  }
  .flex-demo .icon{
    display: inline-block;
    width: 40px;
    height:40px;
    line-height:40px;
    border-radius: 4px;
    color: white;
  }
  .colorAcount1{
    color: #C0B679;
  }
  .colorAcount2{
    color: #52C3A3;
  }
  .colorAcount3{
    color: #F9A133;
  }
</style>

