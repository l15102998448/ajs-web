<!-- 客户案例 -->
<template>
    <div class="case-page">
        <Header activeIndex="/case" :hasBg="true" />
        <div class="case-box">
            <el-row class="editableContent ">
                <h1><span>C</span>USTOMER CASE</h1>
                <p class="text-14 pb-24"><b class="mr-20"></b>客户案例—客户的成功是我们大的荣耀</p>
            </el-row>
        </div>
        <div class="case-list">
                111
        </div>
        <div class="case-list">
                222
        </div>
        <div class="case-list">
                333
        </div>
        <div class="case-list">
                4444
        </div>

        <Footer/>
    </div>
</template>

<script>
import Header from "../components/header.vue"
import Footer from "../components/footer.vue";
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
    components: { Header,Footer }
}
</script>
<style lang="scss" scoped>
/* @import url(); 引入css类 */
@import "../views/otherFile/case"
</style>