<template>
<div>
  <h3>請求管理システム</h3>
  <el-menu default-active="1" @open="handleOpen" @close="handleClose">
    <el-submenu index="1">
      <template slot="title"><span>請求管理</span></template>
      <el-menu-item index="1-1" v-on:click="getStepNumber(); nextTransition()">請求データ登録</el-menu-item>
      <el-menu-item index="1-2">未請求データ処理</el-menu-item>
      <el-menu-item index="1-3">請求済データ処理</el-menu-item>
    </el-submenu>
    <el-submenu index="2">
      <template slot="title"><span>売上管理</span></template>
      <el-menu-item index="2-1">売上データ分析</el-menu-item>
      <el-menu-item index="2-2">売掛データ分析</el-menu-item>
    </el-submenu>
    <el-submenu index="3">
      <template slot="title"><span>登録設定</span></template>
      <el-menu-item index="3-1">顧客</el-menu-item>
      <el-menu-item index="3-2">請求項目</el-menu-item>
    </el-submenu>
  </el-menu>
</div>
</template>

<script>
export default {
  methods: {
    handleOpen (key, keyPath) {
      console.log(key, keyPath)
    },
    handleClose (key, keyPath) {
      console.log(key, keyPath)
    },
    getStepNumber: function (lsStepNumber) {
      window.localStorage.setItem(lsStepNumber, '1')
      this.$store.commit('setStepNumber', lsStepNumber)
    },
    nextTransition () {
      this.$router.push('/')
    }
  }
}
</script>
