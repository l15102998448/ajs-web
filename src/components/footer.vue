<!-- 底部组建 -->
<template>
    <div class="footer">
       <div class="footer-bkg flex-x-between">
           <div>
               <h1>建立安全的信息化系统</h1>
               <p>呵 护 您 的 业 务 及 数 据 健 康 安 全</p>
               <p>Establish a safe and reliable information system to protect the health and safety of your business and data</p>
           </div>
           <div class="img-box"></div>
       </div> 
       <p class="flex-x-center">版权所有 © 某某有限公司</p>
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
    background: yellow;
    .footer-bkg{
        background: rgb(31, 37, 65);
    }
    p{
        background: rgb(18, 22, 43);
    }
}

</style>