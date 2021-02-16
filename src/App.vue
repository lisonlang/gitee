<template>
  <div id="app">
    <div id="nav">
    
      sssssssssssssssssssssssgit chssssssssssssssssssssssssssssssssssssss
    </div>
    <router-view/>
  </div>
</template>

<style lang="less">
.ac{
  color:gray;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
<script>
export default {
  data () {
    return {
      txt:"请输入"
    }
  },
  methods: {
    show(){
      if(this.txt==="请输入")
         this.txt=""

    },
    cshow(){
      if(this.txt===''){
        this.txt='请输入'
      }
    }
  }




}
</script>