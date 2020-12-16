<template>
<div>
  <el-container>
    <el-container>
      <el-aside width="200px" class="invoice-management__aside">
        <allAside></allAside>
      </el-aside>
      <el-main>
        <router-view></router-view>
      </el-main>
    </el-container>
  </el-container>
</div>
</template>

<script>
import allAside from './components/layout/all_aside.vue'

export default {
  components: {
    allAside
  }
}
</script>

<style>
.invoice-management__aside {
  margin: 0 10px;
  border-right: 1px solid #409EFF;
  height: 100vh;
}
</style>
