<template>
  <div id="app">
    <router-view/>
    <Topback></Topback>
  </div>
</template>

<script>
import Topback from "./components/base/Topback";
export default {
  components: {
    Topback
  },
  name: "App"
};
</script>

<style lang="scss">
@import "./assets/css/base_m.css";
@import "element-ui/lib/theme-chalk/display.css";
</style>
