<template>
  <div class="center-layout">
    <div class="inner">xxxxxxx</div>
  </div>
</template>

<style lang="scss">
// display:inline-block,缺点文字对齐不对，而且
/* .center-layout {
  margin-top: 10px;
  height: 400px;
  width: 400px;
  line-height: 400px;
  text-align: center;
  background-color: #f66;
  font-size: 0;
  div {
    display: inline-block;
    vertical-align: middle;
    height: 100px;
    width: 100px;
    background-color: #66f;
  }
} */
.center-layout {
  margin-top: 10px;
  width: 400px;
  height: 400px;
  background-color: #f66;
  .inner {
    width: 100px;
    height: 100px;
    background-color: #66f;
  }
}
// table-cell
/* .center-layout {
  display: table-cell;
  vertical-align: middle;
  .inner {
    margin: 0 auto;
  }
} */
// position
.center-layout {
  position: relative;
  .inner {
    position: absolute;
    top: 50%;
    left: 50%;
    /* margin: -50px 0 0 -50px; */
    // 但是存在一个缺陷，若节点需额外使用transform，那么就比较麻烦了
    transform: translate(-50%, -50%);
  }
}
// flex
.center-layout {
  display: flex;
  .inner {
    margin: auto;
  }
}
</style>

<script>
export default {
  name: "center-layout",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>