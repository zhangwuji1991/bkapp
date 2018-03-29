<template>
  <div>
   <div class="heade">
     个人中心
   </div>
   <nav class="nav">
        <li>
          <router-link :to="{ name: 'topic-create' }" flex="box:justify">
            <div class="icon" flex="cross:center">
              <i class="iconfont icon-edit" style="color: #14b11d"></i>
            </div>
            <div class="text">发表主题</div>
            <div class="arrow">
              <i class="iconfont icon-arrow-right"></i>
            </div>
          </router-link>
        </li>
        <li>
          <router-link :to="{ name: 'self-messages' }" flex="box:justify">
            <div class="icon" flex="cross:center">
              <i class="iconfont icon-msg" style="color: #bd1616;"></i>
            </div>
            <div class="text">我的消息</div>
            <div class="arrow">
              <i class="iconfont icon-arrow-right"></i>
            </div>
          </router-link>
        </li>
      </nav>
  </div>
</template>
<script>
  // import { mapModules } from 'vuet'

  // export default {
  //   mixins: [
  //     mapModules({ self: 'user-self' })
  //   ]
  // }

</script>
<style lang="less" scoped>
 @import "../less/config";
 .heade{
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    height: 50px;
    line-height: 50px;
    border: 1px solid #ddd;
 }
  .nav {
    padding: 0;
    margin-top:  60px;
    li {
      list-style: none;
      border-bottom: 1px solid #ddd;
      background: #fbfbfb;
      &:first-of-type {
        border-top: 1px solid #ddd;
      }
    }
    a {
      padding: 8px 10px;
      line-height: 28px;
      .icon {
        width: 45px;
        .iconfont {
          font-size: 24px;
          color: #aaa;
        }
      }
      .text {
        line-height: 30px;
        font-size: 13px;
        color: @text;
      }
      .icon-arrow-right {
        color: #ccc;
      }
    }
  }
</style>
