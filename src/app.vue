<template>
  <div class="app">
    <quan-p></quan-p>
    <two-side></two-side>
    <three-layout></three-layout>
  </div>
</template>

<script>
import QuanP from "./quanping";
import TwoSide from "./twoside";
import ThreeLayout from "./threelayout";
export default {
  components: {
    QuanP,
    TwoSide,
    ThreeLayout,
  },
};
</script>

<style scoped lang='scss'>
.app {
  display: flex;
  justify-content: space-around;
}
</style>