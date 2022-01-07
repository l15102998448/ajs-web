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
            <div class="banner_con flex-x-between">
                <div class="banner_left">
                    <div class="banner_left_top">
                        <p class="text-16">客户案例—客户的成功是我们大的荣耀</p>
                        <div class="d-flex text-48">HPROPERTY <p class="smBox"></p></div>
                    </div>
                    <div class="mt-40 desc">小屋置业住宅项目的打造，确立了其在上海、广州节能环保科技住宅。小屋置业确立了其在上海、广州节能环保科技住宅。</div>
                </div>
                <div>
                    <img style="display: block; margin-left: 30px" src="../assets/images/banner_01.jpeg" />
                    <img style="display: block;margin-right: 30px" src="../assets/images/banner_02.jpeg" />
                </div>
            </div>
        </div>
        <div class="case-list">
            <div class="banner_con flex-x-between">
                <div class="banner_left">
                    <div class="banner_left_top">
                        <p class="text-16">客户案例—客户的成功是我们大的荣耀</p>
                        <div class="d-flex text-48">HPROPERTY <p class="smBox"></p></div>
                    </div>
                    <div class="mt-40 desc">小屋置业住宅项目的打造，确立了其在上海、广州节能环保科技住宅。小屋置业确立了其在上海、广州节能环保科技住宅。</div>
                </div>
                <div>
                    <img style="display: block; margin-left: 30px" src="../assets/images/banner_01.jpeg" />
                    <img style="display: block;margin-right: 30px" src="../assets/images/banner_02.jpeg" />
                </div>
            </div>
        </div>
        <div class="case-list">
            <div class="banner_con flex-x-between">
                <div class="banner_left">
                    <div class="banner_left_top">
                        <p class="text-16">客户案例—客户的成功是我们大的荣耀</p>
                        <div class="d-flex text-48">HPROPERTY <p class="smBox"></p></div>
                    </div>
                    <div class="mt-40 desc">小屋置业住宅项目的打造，确立了其在上海、广州节能环保科技住宅。小屋置业确立了其在上海、广州节能环保科技住宅。</div>
                </div>
                <div>
                    <img style="display: block; margin-left: 30px" src="../assets/images/banner_01.jpeg" />
                    <img style="display: block;margin-right: 30px" src="../assets/images/banner_02.jpeg" />
                </div>
            </div>
        </div>
        <div class="case-list">
            <div class="banner_con flex-x-between">
                <div class="banner_left">
                    <div class="banner_left_top">
                        <p class="text-16">客户案例—客户的成功是我们大的荣耀</p>
                        <div class="d-flex text-48">HPROPERTY <p class="smBox"></p></div>
                    </div>
                    <div class="mt-40 desc">小屋置业住宅项目的打造，确立了其在上海、广州节能环保科技住宅。小屋置业确立了其在上海、广州节能环保科技住宅。</div>
                </div>
                <div>
                    <img style="display: block; margin-left: 30px" src="../assets/images/banner_01.jpeg" />
                    <img style="display: block;margin-right: 30px" src="../assets/images/banner_02.jpeg" />
                </div>
            </div>
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
