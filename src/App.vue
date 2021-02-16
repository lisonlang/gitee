<template>
  <div id="app">
    <div class="container">
      <div>导航</div>
      <div>导航</div>
      <div>导航</div>
      <div>导航</div>
      <div>导航</div>
      <div>导航</div>
      <div>导航</div>
      <div>导航</div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.container {
  width: 750px;
  display: flex;
  background: green;
  margin: 0px auto;
  div {
    text-align: center;
    flex: auto;
  }
}
@media screen and (max-width: 768px) {
  .container {
    width: 100%;
  display: inline-block;

    div {
      display: inline-block;
      width: 33.3%;
    }
  }
}
</style>
<script>
export default {
  data() {
    return {
      txt: "请输入",
    };
  },
  methods: {
    show() {
      if (this.txt === "请输入") this.txt = "";
    },
    cshow() {
      if (this.txt === "") {
        this.txt = "请输入";
      }
    },
  },
};
</script>