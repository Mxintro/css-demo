<template>
  <div class="text-wrapping">
    <img src="https://static.yangzw.vip/codepen/thor.jpg" />
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
  </div>
</template>

<style lang="scss">
.text-wrapping {
  width: 400px;
  font-size: 20px;
  word-break: break-all;
  color: #f66;
  img {
    float: left;
    width: 200px;
    margin: 10px;
  }
}
</style>

<script>
export default {
  name: "text-wrapping",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>