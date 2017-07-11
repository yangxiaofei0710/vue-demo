<template>
  <div>
     <this-dialog :is-show="isShowCheckDialog"  >
      请检查你的支付状态！
      <div class="button">
        支付成功
      </div>
      <div class="button">
        支付失败
      </div>
    </this-dialog>
    <this-dialog :is-show="isShowSuccessDialog">
      购买成功！
    </this-dialog>
    <this-dialog :is-show="isShowFailDialog">
      购买失败！
    </this-dialog>
  </div>
</template>

<script>
import Dialog from './dialog'
export default {
  components: {
    thisDialog: Dialog
  },
  props: {
    isShowCheckDialog: {
      type: Boolean,
      default: false
    }
  },
  data () {
    return {
      isShowSuccessDialog: false,
      isShowFailDialog: false,
    }
  },
  methods: {
   
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
