<template>
  <div class="three-column-layout">
    <div class="left"></div>
    <div class="center"></div>
    <div class="right"></div>
  </div>
</template>

<style lang="scss">
// flex
/* .three-column-layout {
  display: flex;
  width: 400px;
  height: 400px;
  .left {
    width: 50px;
    background-color: #f66;
  }
  .center {
    width: 100px;
    background: #32cd99;
  }
  .right {
    flex: 1;
    background: #6667ff;
  }
} */

// overflow + float
.three-column-layout {
  width: 400px;
  height: 400px;
  .left {
    float: left;
    width: 50px;
    height: 100%;
    background-color: #f66;
  }
  .center {
    float: left;
    width: 100px;
    height: 100%;
    background: #32cd99;
  }
  .right {
    overflow: hidden;
    height: 100%;
    background: #6667ff;
  }
}
</style>

<script>
// 连续两列宽度固定、剩余一列宽度自适应和三列高度固定且相等
export default {
  name: "threelayout",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>