<template>
   <div class="m-header">
      <div class="navbar">
          <van-icon name="setting-o" size='24'/>
          <van-cell-group>
            <van-field v-model="value"  placeholder="请输入你喜欢的视频名称"  left-icon="search"/>
          </van-cell-group>
         <van-icon name="friends-o" size='24' />
      </div>
      <van-collapse v-model="activeNames">
        <van-collapse-item title="标题1" name="1">内容</van-collapse-item>
      </van-collapse>
   </div>
</template>
<script>
export default {
  data () {
    return {
      value:'',
      activeNames: ['1'],
    }
  }
}
</script>
<style lang="stylus" scoped>
  .m-header {
    width:100%;
    background-color: #fb7299;
    .navbar {
      width 100%
      height: 44px;
      line-height 44px;
      padding: 0 18px
      display flex
      box-sizing border-box
      justify-content space-between
      flex-wrap nowrap
    }
    
  }
</style>
<style lang="stylus" scoped>
  .van-icon-setting-o::before {
    margin-top: 10px;
  }
  .van-icon-friends-o::before {
    margin-top: 10px;
  }
  .van-cell-group {
    background-color: #fb7299;
  }
  .van-cell {
    border-radius 20px;
    color: rgba(255,255,255,0.5);
    background-color: rgba(0,0,0,0.1);
    padding: 5px;
    margin-top: 5px;
  }
</style>