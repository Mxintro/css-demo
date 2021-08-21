<template>
  <div class="app">
    <quan-p></quan-p>
    <two-side></two-side>
  </div>
</template>

<script>
import QuanP from "./quanping";
import TwoSide from "./twoside";
export default {
  components: {
    QuanP,
    TwoSide,
  },
};
</script>

<style scoped lang='scss'>
.app {
  display: flex;
  justify-content: space-around;
}
</style>