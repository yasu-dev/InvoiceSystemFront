<template>
<div class="invoice-management__main0">
  <el-steps :active="$store.state.step_number">
    <el-step title="顧客" icon="el-icon-edit"></el-step>
    <el-step title="商品" icon="el-icon-edit"></el-step>
    <el-step title="手数料" icon="el-icon-edit"></el-step>
    <el-step title="確認" icon="el-icon-view"></el-step>
    <el-step title="登録" icon="el-icon-upload"></el-step>
  </el-steps>
</div>
</template>

<style>
.invoice-management__main0 {
  max-width: 500px;
  position: relative;
}
</style>
