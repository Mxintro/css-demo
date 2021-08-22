<template>
  <div class="grail-layout">
    <div class="left"></div>
    <div class="right"></div>
    <div class="center"><div>qwetrrewrterqwereqwrewrewrewewqrewr</div></div>
  </div>
</template>

<style lang="scss">
// 圣杯布局float + margin-left/right + padding-left/right
/* .grail-layout {
  width: 400px;
  height: 400px;
  padding: 0 100px;
  margin-top: 10px;
  .left {
    float: left;
    width: 100px;
    height: 100%;
    margin-left: -100px;
    background-color: #f66;
  }
  .right {
    float: right;
    width: 100px;
    height: 100%;
    margin-right: -100px;
    background-color: #66f;
  }
  .center {
    height: 100%;
    background-color: #3c9;
  }
} */
// 双飞翼布局float + margin-left/right
.grail-layout {
  width: 400px;
  height: 400px;
  margin-top: 10px;
  .left {
    float: left;
    width: 100px;
    height: 100%;
    background-color: #f66;
  }
  .right {
    float: right;
    width: 100px;
    height: 100%;
    background-color: #66f;
  }
  .center {
    margin: 0 100px;
    height: 100%;
    background-color: #3c9;
  }
}
</style>

<script>
export default {
  name: "grail-layout",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>