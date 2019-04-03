<template>
  <div class="swiper">
    <div class="block">
      <el-carousel :interval="4000" trigger="click" height="20rem">
        <el-carousel-item v-for="item in 3" :key="item">
          <h3>{{ item }}</h3>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
export default {
  name: "Swiper",
  data() {
    return {};
  }
};
</script>

<style scoped lang="scss">
.el-carousel{
  border-radius: 4px;
}
//轮播图
.el-carousel__item h3 {
  color: #475669;
  font-size: 14px;
  opacity: 0.75;
  line-height: 150px;
  margin: 0;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>
