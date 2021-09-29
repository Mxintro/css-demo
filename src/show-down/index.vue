<template>
  <div class="component-once-show">
    <span class="label">这是一段文字</span>
    <div class="content-list" tabindex="-1">
      <div class="list-item">1</div>
      <div class="list-item">2</div>
      <div class="list-item">3</div>
      <div class="list-item">4</div>
      <div class="list-item">5</div>
      <div class="list-item">6</div>
    </div>
  </div>
</template>

<style lang="scss">
.component-once-show {
  width: 200px;
  height: 30px;
  margin: 30px;
  line-height: 30px;
  border: 1px solid #eeeeee;
  border-radius: 3px;
  text-align: center;
  box-shadow: 0 0 5px 2px #eeeeee;
  position: relative;
}
.content-list {
  visibility: hidden;
  position: absolute;
  width: 100%;
  border: 0px solid;
  border-radius: 3px;
  box-shadow: 0 0 5px 2px #eeeeee;
  margin-top: 5px;
  outline: none;
}

.component-once-show .content-list:focus {
  visibility: visible;
}

.component-once-show .label:hover + .content-list {
  visibility: visible;
}

.component-once-show .content-list:focus {
  visibility: visible;
}

.component-once-show .content-list:hover {
  visibility: visible;
}

.component-once-show .content-list .list-item {
  background: #ffffff;
  height: 30px;
  line-height: 30px;
  transition: background 0.8s ease-out;
}

.component-once-show .content-list .list-item:hover {
  background: #eeeeee;
}
</style>

<script>
export default {
  name: "show-down",
  props: {
    done: {
      default: "Done",
      type: String,
    },
  },
};
</script>