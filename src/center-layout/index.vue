<template>
  <div class="center-layout">
    <div>xxxxxxx</div>
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
  display: table-cell;
  vertical-align: middle;
  div {
    width: 100px;
    height: 100px;
    background-color: #66f;
    margin: auto;
  }
}
// table-cell
/* .center-layout {
  display: table-cell;
  vertical-align: middle;
  text-align: center;
  div {
    margin: auto;
  }
} */
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