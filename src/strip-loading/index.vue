<template>
  <div class="strip-loading-component">
    <ul class="strip-loading">
      <li v-for="v in 6" :key="v" :style="`--line-index: ${v}`"></li>
    </ul>
  </div>
</template>

<style lang="scss">
.strip-loading-component {
  margin: 100px;
  .strip-loading {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 200px;
    height: 200px;
    // 普通写法
    /* li {
      border-radius: 3px;
      width: 6px;
      height: 30px;
      background-color: #f66;
      animation: beat 1s ease-in-out infinite;
      // 技巧：除第一个外，后面的都加margin
      & + li {
        margin-left: 5px;
      }
      // :nth-child(n) 选择器匹配属于其父元素的第 N 个子元素，不论元素的类型。
      &:nth-child(2) {
        animation-delay: 200ms;
      }
      &:nth-child(3) {
        animation-delay: 400ms;
      }
      &:nth-child(4) {
        animation-delay: 600ms;
      }
      &:nth-child(5) {
        animation-delay: 800ms;
      }
      &:nth-child(6) {
        animation-delay: 1s;
      }
    } */
    li {
      --time: calc((var(--line-index)-1) * 200ms);
      border-radius: 3px;
      width: 6px;
      height: 30px;
      background-color: #f66;
      animation: beat 1s ease-in-out infinite;
      animation-delay: var(--time);
      /* animation-delay: calc((var(--line-index)-1) * 200ms);/ 这样出错，可能是打包出错 */
      & + li {
        margin-left: 5px;
      }
    }
  }
  @keyframes beat {
    0%,
    100% {
      transform: scaleY(1);
    }
    50% {
      transform: scaleY(0.5);
    }
  }
}
</style>

<script>
export default {
  name: "strip-loading",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>