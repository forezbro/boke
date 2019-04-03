<template>
  <div class="message">
    <h2>其他推荐</h2>
    <div class="msg-box">
      <div class="msg-title ell-1">作为一个设计师,如果遭到质疑你是否能恪守自己的原则?</div>
      <div class="msg-info fx fx-y-center">
        <div class="msg-info-img">
          <img src="../../assets/logo.png" alt>
        </div>
        <div>
          <p
            class="ell-3"
          >就拿我自己来说吧，有时候会很矛盾，设计好的作品，不把它分享出来，会觉得待在自己电脑里面实在是没有意义。干脆就发布出去吧。我也害怕收到大家不好的评论，有些评论，可能说者无意，但是对于每一个用心的站长来说，都会受很深</p>
          <div class="msg-more fx fx-x-between">
            <span>2018.12.45</span>
            <span class="more-btn">阅读更多</span>
          </div>
        </div>
      </div>
    </div>
    <div class="msg-box">
      <div class="msg-title ell-1">作为一个设计师,如果遭到质疑你是否能恪守自己的原则?</div>
      <div class="msg-info fx fx-y-center">
        <div class="msg-info-img">
          <img src="../../assets/logo.png" alt>
        </div>
        <div>
          <p
            class="ell-3"
          >就拿我自己来说吧，有时候会很矛盾，设计好的作品，不把它分享出来，会觉得待在自己电脑里面实在是没有意义。干脆就发布出去吧。我也害怕收到大家不好的评论，有些评论，可能说者无意，但是对于每一个用心的站长来说，都会受很深</p>
          <div class="msg-more fx fx-x-between">
            <span>2018.12.45</span>
            <span class="more-btn">阅读更多</span>
          </div>
        </div>
      </div>
    </div>
    <div class="msg-box">
      <div class="msg-title ell-1">作为一个设计师,如果遭到质疑你是否能恪守自己的原则?</div>
      <div class="msg-info fx fx-y-center">
        <div class="msg-info-img">
          <img src="../../assets/logo.png" alt>
        </div>
        <div>
          <p
            class="ell-3"
          >就拿我自己来说吧，有时候会很矛盾，设计好的作品，不把它分享出来，会觉得待在自己电脑里面实在是没有意义。干脆就发布出去吧。我也害怕收到大家不好的评论，有些评论，可能说者无意，但是对于每一个用心的站长来说，都会受很深</p>
          <div class="msg-more fx fx-x-between">
            <span>2018.12.45</span>
            <span class="more-btn">阅读更多</span>
          </div>
        </div>
      </div>
    </div>
    <div class="msg-box">
      <div class="msg-title ell-1">作为一个设计师,如果遭到质疑你是否能恪守自己的原则?</div>
      <div class="msg-info fx fx-y-center">
        <div class="msg-info-img">
          <img src="../../assets/logo.png" alt>
        </div>
        <div>
          <p
            class="ell-3"
          >就拿我自己来说吧，有时候会很矛盾，设计好的作品，不把它分享出来，会觉得待在自己电脑里面实在是没有意义。干脆就发布出去吧。我也害怕收到大家不好的评论，有些评论，可能说者无意，但是对于每一个用心的站长来说，都会受很深</p>
          <div class="msg-more fx fx-x-between">
            <span>2018.12.45</span>
            <span class="more-btn">阅读更多</span>
          </div>
        </div>
      </div>
    </div>
    <div class="more hidden-sm-and-up">
      查看更多
    </div>
    <div class="block fx fx-x-center hidden-xs-only">
      <el-pagination
        @size-change="handleSizeChange"
        @current-change="handleCurrentChange"
        :current-page.sync="currentPage1"
        :page-size="1"
        layout="total, prev, pager, next"
        :total="20"
      >
        <p>2424242424</p>
        <p>2424242424</p>
        <p>2424242424</p>
      </el-pagination>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    handleSizeChange(val) {
      console.log(`每页 ${val} 条`);
    },
    handleCurrentChange(val) {
      console.log(`当前页: ${val}`);
    }
  },
  data() {
    return {
      currentPage1: 5
    };
  }
};
</script>

<style scoped lang="scss">
.message {
  margin-top: 1rem;
  padding: 1rem;
  box-shadow: 0px 0px 3px 0px #ccc;
  background: white;
  .more{
    font-size: 1.4rem;
    cursor: pointer;
    padding: 0.4rem 0.6rem;
    border: 1px solid #ccc;
    display: inline-block;
    margin-top: 1.6rem;
    border-radius: 8px;
    transition: all .3s linear;
  }
  .more:hover{
    background: #409eff;
    color: white;
  }
  .block{
    margin: 1rem 0;
  }
  h2 {
    padding: 1rem 0 1rem 0;
    font-size: 2rem;
    border-bottom: 1px solid #ccc;
  }
  .msg-box:hover .msg-title {
    color: #409eff;
  }
  .msg-box {
    border-bottom: 1px solid #ccc;
    padding-bottom: 2rem;
    margin-top: 1rem;
    cursor: pointer;
    .msg-title {
      font-weight: bold;
      font-size: 1.6rem;
      margin: 1rem 0;
      transition: all 0.3s linear;
    }
    .msg-info-img {
      margin-right: 2rem;
      border-radius: 4px;
      height: 10rem;
      width: 26rem;
      border-radius: 4px;
      img {
        width: 100%;
        height: 100%;
      }
    }
    .msg-more {
      margin-top: 3rem;
    }
    p {
      color: #666;
      text-indent: 2rem;
      font-size: 1.4rem;
    }
    .more-btn {
      padding: 0.6rem 0.8rem;
      background: #409eff;
      color: white;
      font-size: 1.4rem;
      border-radius: 8px;
    }
  }
}
</style>
