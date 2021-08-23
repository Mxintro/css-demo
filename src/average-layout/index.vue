<template>
  <div class="average-layout">
    <div class="one"></div>
    <div class="two"></div>
    <div class="three"></div>
    <div class="four"></div>
  </div>
</template>

<style lang="scss">
.average-layout {
  display: flex;
  height: 400px;
  width: 400px;
  > div {
    flex: 1;
  }
  .one {
    background-color: #f66;
  }
  .two {
    background-color: #66f;
  }
  .three {
    background-color: #f90;
  }
  .four {
    background-color: #09f;
  }
}
</style>

<script>
export default {
  name: "average-layout",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>