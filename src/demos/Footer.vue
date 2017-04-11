<template>
  <tabbar class="footer" icon-class="icon"  slot="bottom">
    <tabbar-item v-for="lab in footerLabs" :key="lab.id" :link="lab.link">
      <span :class="lab.class" slot="icon" style=""></span>
      <span slot="label" v-html="lab.lab"></span>
    </tabbar-item>
  </tabbar>
</template>
<script>
  import { Tabbar, TabbarItem } from 'vux'
  import { mapState, mapActions } from 'vuex'

  export default {
    components: {
      Tabbar,
      TabbarItem,
      mapState,
      mapActions
    },
    data () {
      return {
        footerLabs: [{ id: 1, lab: '首页', class: 'i-a01a', link: '/' }, { id: 2, lab: '护理员', class: 'i-tianjiahuiyuan', link: '/info' }, { id: 3, lab: '订单', class: 'i-order', link: '/' }, { id: 4, lab: '我的', class: 'i-kehu', link: '/MyDemo' }],
        isTabbarDemo: false
      }
    }
  }
</script>
<style scoped>
  @import '~vux/src/styles/iconfont.less';
  .footer{
    background: white;
    width: 100%;
    line-height:1;
  }
</style>
