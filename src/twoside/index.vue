<template>
  <div class="two-column-layout">
    <div class="left"></div>
    <div class="right"></div>
  </div>
</template>

<style lang="scss">
// flex
/* .two-column-layout {
  display: flex;
  height: 400px;
  width: 400px;
  .left {
    width: 100px;
    background-color: #f66;
  }
  .right {
    flex: 1;
    background: #32cd99;
  }
} */
// float + margin-left/right
/* .two-column-layout {
  height: 400px;
  width: 400px;
  .left {
    float: left;
    width: 100px;
    height: 100%;
    background-color: #f66;
  }
  .right {
    margin-left: 100px;
    height: 100%;
    background: #32cd99;
  }
} */
//
.two-column-layout {
  height: 400px;
  width: 400px;
  .left {
    float: left;
    width: 100px;
    height: 100%;
    background-color: #f66;
  }
  .right {
    margin-left: 100px;
    height: 100%;
    background: #32cd99;
  }
}
</style>

<script>
export default {
  name: "twoside",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>