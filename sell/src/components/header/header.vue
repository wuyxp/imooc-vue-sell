<template>
  <div :class="{header:true,'v-class':true}">
    <div class="content-wrapper">
      <div class="avatar">
        <img :src="seller.avatar" width="64" height="64" alt="">
      </div>
      <div class="content">
        <div class="title">
          <span class="brand"></span>
          <span class="name"></span>
        </div>
      </div>
      <div class="description">

      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'v-header',
  props:{
    seller:{
      type: Object
    },
    'v-class':{
      type: String
    }
  }
}
</script>

<style lang="stylus" scoped>
 .avatar
  border: 1px solid red
  img
    border: 1px solid green
</style>


