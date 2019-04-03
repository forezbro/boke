<template>
  <div class="footer">
      <div class="fx fx-x-around fx-y-center">
          <div>
              <div class="photo"><img src="../../assets/me.jpg" alt=""></div>
              <p class="fx fx-x-center">我的微信</p>
          </div>
          <div>
              <h2>站点声明</h2>
              <p>1、本站个人博客模板，均为七步本人设计，个人可以使用，但是未经许可不得用于任何商业目的。</p>
              <p>2、所有文章未经授权禁止转载、摘编、复制或建立镜像，如有违反，追究法律责任。举报邮箱：1076613617@qq.com</p>
              <p>Copyright © www.yangqq.com All Rights Reserved. 备案号：蜀ICP备11002373号-1</p>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {};
  }
};
</script>

<style scoped lang="scss">
.footer{
    margin-top: 2rem;
    padding: 2rem 0;
    background: #373D41;
    color: #73777a;
    .photo{
        width: 8rem;
        height: 8rem;
        img{
            width: 100%;
            height: 100%;
        }
    }
    h2{
        font-size: 2rem;
        margin: 0rem 0 0.8rem;
        color: #409eff;
    }
    p{
        font-size: 1.2rem;
    }
}
</style>
