<template>
  <div class="app">
    <!-- <center-layout></center-layout> -->
    <!-- <text-wrapping></text-wrapping> -->
    <text-ellipis />
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