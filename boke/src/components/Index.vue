<template>
  <div class="index">
    <Tabbar></Tabbar>
    <el-row :gutter="6" style="margin:0">
      <div class="info">
        <el-col :sm="16" :md="18">
          <div class="l-info">
            <Swiper></Swiper>
            <Skill></Skill>
            <Message></Message>
          </div>
        </el-col>
        <el-col :sm="8" :md="6" class="hidden-xs-only">
          <div  class="r-info">
            <div class="my-info">
              <h2>我的名片</h2>
              <p>名称：Forez | 七步</p>
              <p>职业：web前端工程师</p>
              <p>现居：重庆市-九龙坡</p>
              <p>Email：1076613617@qq.com</p>
              <div class="fx fx-x-around" style="margin-top:1.2rem">
                <a href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=1076613617@qq.com">
                  <i class="icon iconemail"></i>
                </a>
                <el-tooltip class="item" effect="dark" content="微信号：qwe2133927" placement="top">
                      <i class="icon iconweixin"></i>
                </el-tooltip>
                <a
                  href="http://shang.qq.com/open_webaio.html?sigt=07403c52f577c13aaed85bd5cfeb78bb8a9169f241fa87ba0fb19000278e9b6dc1a8cbe244247c2d368ab49ddbd1330c&sigu=fd734225f5aa4d6ebf26e7712724c98c186fd3a259076de519b1aed9b95ec82670650c02187f766c&tuin=1076613617"
                >
                  <i class="icon iconqq"></i>
                </a>
              </div>
            </div>
            <div class="updata">
              <h2>
                最近更新
                <div class="line"></div>
              </h2>
              <ul>
                <li class="ell-1">双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦</li>
                <li class="ell-1">双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦</li>
                <li class="ell-1">双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦</li>
                <li class="ell-1">双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦</li>
              </ul>
            </div>
            <div class="updata top-click">
              <h2>
                点击最多
                <div class="line"></div>
                <div class="click-img">
                  <img src="../assets/click.jpg" alt>
                </div>
              </h2>
              <ul>
                <li class="ell-1">
                  <span>1</span>双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦
                </li>
                <li class="ell-1">
                  <span>2</span>双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦
                </li>
                <li class="ell-1">
                  <span>3</span>双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦
                </li>
                <li class="ell-1">
                  <span>4</span>双十一，阿里云特惠活动，快来领券啦双十一，阿里云特惠活动，快来领券啦
                </li>
              </ul>
            </div>
          </div>
        </el-col>
      </div>
    </el-row>
    <Footer></Footer>
  </div>
</template>

<script>
import Tabbar from "./base/Tabbar";
import Swiper from "./base/Swiper";
import Skill from "./base/Skill";
import Message from "./base/Message";
import Footer from "./base/Footer";
export default {
  components: {
    Tabbar,
    Swiper,
    Skill,
    Message,
    Footer
  },
  name: "Index",
  data() {
    return {};
  }
};
</script>

<style scoped lang="scss">
i {
  font-size: 3rem;
  color: white;
}
.info {
  width: 80%;
  margin: 1rem auto 0;
}
.r-info {
  margin-left: 1rem;
  .my-info {
    color: white;
    background: url(../assets/bg.jpg) no-repeat;
    background-size: cover;
    height: 20rem;
    border-radius: 4px;
    p {
      font-size: 1.3rem;
      margin-left: 2rem;
      padding-top: 1rem;
    }
    h2 {
      font-size: 2rem;
      margin-left: 1rem;
      padding-top: 1rem;
      padding-bottom: 1rem;
    }
  }
  .updata {
    background: url(../assets/bj1.jpg) no-repeat;
    background-size: cover;
    padding: 1rem 0 2rem;
    border-radius: 4px;
    margin-top: 1rem;
    h2 {
      font-weight: normal;
      font-size: 1.6rem;
      border-bottom: 1px solid #ccc;
      margin: 0 1rem;
      padding: 1rem 0;
      position: relative;
      padding-bottom: 1rem;
      cursor: pointer;
      .line {
        top: 3.6rem;
        width: 30%;
      }
    }
    :hover .line {
      width: 100%;
    }
    ul {
      width: 80%;
      margin: 0 auto;
      :hover {
        font-weight: bold;
      }
      li {
        margin: 1rem 0;
        font-size: 1.4rem;
        cursor: pointer;
        color: rgba(0, 0, 0, 0.92);
        transition: all 0.3s linear;
      }
    }
  }
  .top-click {
    background: white;
    border: 1px solid #ccc;
    span {
      display: inline-block;
      margin-right: 1rem;
      padding: 0.2rem 0.4rem;
      color: white;
      background: #ccc;
    }
    .click-img {
      margin-top: 2rem;
      img {
        width: 100%;
        height: 100%;
      }
    }
    ul {
      background: url(../assets/bj2.jpg) no-repeat;
      padding: 1rem 1rem 2rem;
      background-size: cover;
      :hover {
        transform: scale(1.1);
      }
      li {
        color: rgba(0, 0, 0, 0.92);
        transition: all 0.3s linear;
        font-size: 1.2rem;
      }
    }
  }
}
</style>
