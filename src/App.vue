<template>
  <div id="app">
    <div id="nav">
      <div class="d1">1</div>
      <div class="d2">2</div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.d1 {
    flex: auto;
    background: red;
  }
  .d2 {
    flex: auto;
    background: pink;
  }

@media screen and (max-width: 800px) {
  #nav {
    display: block;
  }
 
}
@media screen and (min-width: 801px) {
  #nav {
    display: flex;
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