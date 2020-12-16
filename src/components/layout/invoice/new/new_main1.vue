<template>
<div>
  <p><textClient tagname="顧客名"></textClient></p>
  <p><el-link type="warning">顧客登録はこちら</el-link></p>
  <p><buttonRegistration1 class="order-management__button1" tagname="商品情報入力 >"></buttonRegistration1></p>
</div>
</template>

<script>
import textClient from '../../../parts/invoice/new/text_client.vue'
import buttonRegistration1 from '../../../parts/invoice/new/button_registration1.vue'

export default {
  components: {
    textClient,
    buttonRegistration1
  }
}
</script>

<style>
.order-management__button1 {
  line-height: 100px;
}
</style>
