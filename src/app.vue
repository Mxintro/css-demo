<template>
  <div class="app">
    <!-- <center-layout></center-layout> -->
    <!-- <text-wrapping></text-wrapping> -->
    <!-- <text-ellipis /> -->
    <!-- <func-attr></func-attr> -->
    <func-counter></func-counter>
  </div>
</template>

<script>
import QuanP from "./quanping";
import TwoSide from "./twoside";
import ThreeLayout from "./threelayout";
import GrailLayout from "./grail-layout";
import AverageLayout from "./average-layout";
import CenterLayout from "./center-layout";
import TextWrapping from "./text-wrapping";
import TextEllipis from "./text-ellipsis";
import FuncAttr from "./func-attr";
import FuncCounter from "./func-counter";
export default {
  components: {
    QuanP,
    TwoSide,
    ThreeLayout,
    GrailLayout,
    AverageLayout,
    CenterLayout,
    TextWrapping,
    TextEllipis,
    FuncAttr,
    FuncCounter,
  },
};
</script>

<style scoped lang='scss'>
/* .app {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  align-content: space-around;
} */
</style>