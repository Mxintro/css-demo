<template>
  <div class="app">
    <!-- <quan-p></quan-p>
    <two-side></two-side>
    <three-layout></three-layout>
    <grail-layout></grail-layout>
    <average-layout></average-layout> -->
    <center-layout></center-layout>
  </div>
</template>

<script>
import QuanP from "./quanping";
import TwoSide from "./twoside";
import ThreeLayout from "./threelayout";
import GrailLayout from "./grail-layout";
import AverageLayout from "./average-layout";
import CenterLayout from "./center-layout";
export default {
  components: {
    QuanP,
    TwoSide,
    ThreeLayout,
    GrailLayout,
    AverageLayout,
    CenterLayout,
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