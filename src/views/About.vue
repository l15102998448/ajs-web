<template>
  <div class="home-box">
    <el-divider />
    <div class="home">
      <div class="home_top flex-x-between flex-y-center">
        <img src="../assets/images/logo.png"/>
        <el-menu :default-active="activeIndex" 
          class="el-menu-demo"
          mode="horizontal"
          text-color="#fff"
          active-text-color="#ff5c35"
         @select="handleSelect">
          <el-menu-item v-for="(item,index) in titleList" :index="item.value" :key="index">{{item.label}}</el-menu-item>
        </el-menu>
      </div>
      <div class="w-banner-content">
        <div class="smartAbs">
          <div class="smAreaC"></div>
          <div class="editableContent_01">Asian Technology Platform(A. T. P)</div>
          <div class="editableContent_02">your best choose</div>
          <div class="editableContent_04">亚经讯，您的最佳合作伙伴</div>
          <div class="editableContent_03 text-16"><span style="font-family:Source Han Sans,Geneva,sans-serif">一站式服务&nbsp; 客户的成功是我们大的荣耀</span></div>
        </div>
      </div>
      
    </div>
    <div class="content_desc">
      哎哎哎啊
    </div>
    <Footer/>
  </div>
</template>

<script>
import Footer from "../components/footer.vue";
export default {
    name: "Home",
    components: { Footer },
    data() {
      return {
        activeIndex:"1",
        titleList: [
          { value: "1" , label: '首页'},
          { value: "2" , label: '关于我们'},
          { value: "3" , label: '客户案例'},
          { value: "4", label: '新闻资讯'},
          { value: "5" , label: '我们的服务'},
          { value: "6" , label: '联系我们'},
        ]
      }
    },
    methods: {
      handleSelect(val){
        console.log('val',val)
      }
    }
}
</script>
<style lang="scss" scoped>
@import './home'

</style>