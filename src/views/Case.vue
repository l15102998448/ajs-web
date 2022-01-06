<!-- 客户案例 -->
<template>
    <div style="background-color: aquamarine;">case
        <Header activeIndex="/case" />
    </div>
</template>

<script>
import Header from "../components/header.vue"
export default {
    data() {
        return {};
    },
    //生命周期 - 创建完成（访问当前this实例）
    created() {
    },
    //生命周期 - 挂载完成（访问DOM元素）
    mounted() {
    },
    components: { Header }
}
</script>
<style scoped>
/* @import url(); 引入css类 */

</style>