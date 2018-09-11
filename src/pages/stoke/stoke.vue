<template>
  <div id="app">
    <div class = "mui-bar mui-bar-nav">
      <top pagetitle="库存查询" />
      <form id='login-form' class="mui-input-group">
        <div class="mui-input-row">
          <label>区域</label>
          <label>请选择区域</label>
          <label class="mui-navigate-right"></label>
        </div>
        <div class="mui-input-row">
          <label>仓库</label>
          <label>请选择仓库</label>
          <label class="mui-navigate-right"></label>
        </div>
      </form>
    </div>
    <div class="mui-content">
        <liststoke />
    </div>
  
    <bottom />
  </div>
</template>

<script>
  import top from "../../components/top"
  import liststoke from '../stoke/list_stoke'
  import bottom from "../../components/bottom"
  export default {
    components: {
      top,
      liststoke,
      bottom
    }
  }
</script>

<style scoped>
  .mui-content {
    margin-top: 80px;
    margin-bottom: 50px;
  }
  .mui-bar {
    padding-left: 0;
    padding-right: 0;
  }
</style>