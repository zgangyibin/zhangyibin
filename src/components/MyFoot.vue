<template>
    <div class="my-foot">
        <div class="custom-control custom-checkbox">
              <input type="checkbox" class="form-check-input" id="footercheckbox">
              <label for="footercheckbox" class="custom-control-label">全选</label>
        </div>
        <!-- 合计 -->
        <div>
            <span>合计</span>
            <span class="price">￥0</span>
        </div>
        <!-- 结算 -->
        <button type="button" class="footer-btn btn btn-primary">结算(0</button>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="less" scoped>
.my-foot{
    position: fixed;
    z-index: 2;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 50px;
    border-top: 1px solid #ccc;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 10px;
    background-color: #fff;
    .price {
        color: red;
        font-weight: bold;
        font-size: 14px;
    }
    .footer-btn {
        min-width: 80px;
        height: 30px;
        line-height: 30px;
        border-radius: 25px;
        padding: 0;
    }
}
</style>