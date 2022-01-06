<template>
  <div class="about-box">
    <Header activeIndex="/about" :hasBg="true" />
    <div class="about-container">
        <el-row class="editableContent mb-40">
          <h1><span>A</span>BOUT US</h1>
          <p class="text-14"><b class="mr-20"></b>我们的故事—客户的成功是我们大的荣耀</p>
        </el-row>
        <div class="company-profile">
            <h1 class="text-14 mb-20">COMPANY PROFILE</h1>
            <p>秉承以专业、用心的态度为用户提供真诚的服务</p>
            <div class="my-20 text-14">创建于2021年11月23日，迄今为止在网站建设行业已经服务了12年，为北京和全国各地用户提供了专业网站建设服务，及网站建设解决方案。提供专业的网页设计、传统定制建设网站、域名空间等服务，秉承以专业、用心的态度为用户提供真诚的服务。我们深信只要达到每一位用户的要求，就会被认可，从而与我们长期合作，这样，我们也可以走得更远！</div>
            <ul class="py-20 flex-x-between">
              <li>
                <p class="smBox"></p>
                <h3>1000+</h3>
                <div class="text-14">各领域的合作客户</div>
              </li>
               <li>
                <p class="smBox "></p>
                <h3>1年</h3>
                <div class="text-14">专注企业网络营销实践</div>
              </li>
               <li>
                <p class="smBox "></p>
                <h3>95%</h3>
                <div class="text-14">客户续费率</div>
              </li>
            </ul>
        </div>
    </div>
    <div class="cutures-box">
      <div class="cutures-container">
        <el-row class="flex-x-center flex-column">
          <h1><span>C</span>ORPORATE CULTURES</h1>
          <p class="text-14 mt-12 mb-44">我们的企业文化</p>
        </el-row>
        <ul class="flex-x-between">
          <li>
            <img src="../assets/images/about_01.png"/>
            <strong>服务理念</strong>
            <p>合作有起点，服务无止境</p>
          </li>
          <li>
            <img src="../assets/images/about_01.png"/>
            <strong>经营理念</strong>
            <p>合作有起点，服务无止境</p>
          </li>
          <li>
            <img src="../assets/images/about_01.png"/>
            <strong>设计理念</strong>
            <p>用心设计每一个网站</p>
          </li>
          <li>
            <img src="../assets/images/about_01.png"/>
            <strong>管理理念</strong>
            <p>领导有权限，管理无界限</p>
          </li>
        </ul>
      </div>
    </div>
    <div class="partners-box">
      <div class="partners-container py-100">
          <el-row class="flex-x-center flex-column">
          <h1><span>P</span>ARTNERS</h1>
          <p class="text-14 mt-12 mb-44">合作伙伴</p>
        </el-row>
        <div class="slideshow">
          <div class="images">
              <img v-for="item in 4" :key="item" src="../assets/images/about_05.png" />
              <img v-for="item in 6" :key="item" src="../assets/images/about_06.png" />
              <img v-for="item in 4" :key="item" src="../assets/images/about_05.png" />
              <img v-for="item in 6" :key="item" src="../assets/images/about_06.png" />
              <img v-for="item in 4" :key="item" src="../assets/images/about_05.png" />
              <img v-for="item in 6" :key="item" src="../assets/images/about_06.png" />
          </div>
        </div>
      </div>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Footer from "../components/footer.vue";
import Header from "../components/header.vue";
export default {
    name: "Home",
    components: { Footer, Header },
    data() {
      return {
        
      }
    },
    methods: {
    
    }
}
</script>
<style lang="scss" scoped>
@import '../views/otherFile/about.scss'

</style>