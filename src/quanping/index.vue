<template>
  <!--  三部分左右满屏拉伸、顶部底部高度固定和主体高度自适应 -->
  <div class="fullscreen-layout">
    <header></header>
    <main></main>
    <footer></footer>
  </div>
</template>

<style lang="scss">
/* position + left/right... */
/* .fullscreen-layout {
  position: relative;
  width: 200px;
  height: 400px;

  header,
  main,
  footer {
    position: absolute;
    left: 0;
    right: 0;
  }
  header {
    top: 0;
    height: 50px;
    background-color: #f66;
  }
  main {
    top: 50px;
    bottom: 50px;
    background: #32cd99;
  }
  footer {
    bottom: 0;
    height: 50px;
    background: #6667ff;
  }
} */
.fullscreen-layout {
  display: flex;
  flex-direction: column;
  width: 200px;
  height: 400px;

  header,
  main,
  footer {
  }
  header {
    height: 50px;
    background-color: #f66;
  }
  main {
    flex: 1;
    background: #32cd99;
  }
  footer {
    height: 50px;
    background: #6667ff;
  }
}
</style>

<script>
export default {
  name: "quanping",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>