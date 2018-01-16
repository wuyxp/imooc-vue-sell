<template>
  <div id="app" class="app">
    <v-header>

    </v-header>
    <div class="tab border-1px">
      <div class="tab-item">
        <router-link to="/goods">
          商品
        </router-link>
      </div>
      <div class="tab-item">
        <router-link to='/ratings'>  
          评论
        </router-link>
      </div>
      <div class="tab-item">
        <router-link to='/seller'>
          商家
        </router-link>
      </div>
    </div>
    <div class="content">
      <router-view>
        
      </router-view>
    </div>
  </div>
</template>

<script>
import header from '@/components/header/header.vue';

export default {
  name: 'app',
  components: {
    'v-header': header
  }
}
</script>

<style lang='stylus'>
  @import "./common/stylus/mixin.styl"
  #app
    .tab
      display: flex
      height : 40px
      width: 100%
      line-height : 40px
      .tab-item
        flex: 1
        text-align: center
        border-1px(rgba(17, 17, 27, 0.1))
        & > a
          display: block
          font-size: 14px
          color: rgb(77, 85, 93)
          &.active
            color: rgb(240, 20, 20)
</style>
