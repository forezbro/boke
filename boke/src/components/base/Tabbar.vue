<template>
  <div class="tabbar">
    <div :class="navBarFixed == true ? 'navBarWrap' :''" class="fx fx-x-around">
      <div class="tab-logo">
        <img src="../../assets/logo.png">
      </div>
        <ul class="fx fx-y-center">
          <li>
            <span>
              网站首页
              <div class="line"></div>
            </span>
          </li>
          <li>
            <span>
              技术文档
              <div class="line"></div>
            </span>
          </li>
          <li>
            <span>
              时间轴
              <div class="line"></div>
            </span>
          </li>
          <li>
            <span>
              留言板块
              <div class="line"></div>
            </span>
          </li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Tabbar",
  data() {
    return {
      navBarFixed: false
    };
  },
  mounted() {
    // 事件监听滚动条
    window.addEventListener("scroll", this.watchScroll);
  },
  methods: {
    watchScroll() {
      var scrollTop =
        window.pageYOffset ||
        document.documentElement.scrollTop ||
        document.body.scrollTop;
      //  当滚动超过 50 时，实现吸顶效果
      if (scrollTop > 50) {
        this.navBarFixed = true;
      } else {
        this.navBarFixed = false;
      }
    }
  }
};
</script>

<style scoped lang="scss">
.navBarWrap {
  transition: all 0.3s linear;
  position: fixed;
  top: 0;
  width: 100%;
  background: #eee;
  z-index: 999;
}
.tabbar {
  .tab-logo {
    width: 6rem;
    height: 6rem;
    img {
      width: 100%;
      height: 100%;
    }
  }
  background: rgb(248, 248, 248);
  ul {
    li {
      cursor: pointer;
      padding: 0 2rem;
      :hover {
        color: #333;
      }
      :hover div {
        width: 100%;
      }
      span {
        font-size: 1.5rem;
        color: #696969;
        position: relative;
        font-weight: bold;
        transition: all 0.3s linear;
      }
    }
  }
}
</style>
