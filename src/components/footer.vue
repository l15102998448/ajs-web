<!-- 底部组建 -->
<template>
    <div class="footer">
        <div class="footer-bkg flex-x-between text-14">
            <p>一站式服务  客户的成功是我们大的荣耀</p>
            <p class="flex-x-center">版权所有 © 亚经讯有限公司</p>
        </div> 
        <div class="footer-bottom text-12">
            <span>本网站支持 &nbsp; | &nbsp; IPv6 &nbsp; | &nbsp; Powered by CloudDream</span>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {

        }
    },
    //生命周期 - 创建完成（访问当前this实例）
    created() {

    },
    //生命周期 - 挂载完成（访问DOM元素）
    mounted() {

    }
}
</script>
<style lang="scss" scoped>
.footer{
    background: rgb(34, 34, 34);
    .footer-bkg{
        width: 80%;
        margin: 0 auto;
    }
    p{
        color:#aaaaaa;
        line-height: 60px;
    }
    .footer-bottom{
        background: #fff;
    }
}

</style>