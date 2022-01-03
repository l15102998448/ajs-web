<template>
  <div class="home-box">
    <el-divider />
    <Header />
    <div class="home">
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
      <div class="home">
        <div class="desc_top">
          <p class="text-16">我们的优势—选择我们的理由</p>
          <div class="d-flex text-48">ADVANTAGE <p class="smBox"></p></div>
        </div>
        <div class="desc_con mt-80">
          <div class="desc_con_item">
            <div class="con_item_left">
              <p class="text-20">多年专注</p>
              <p class="my-12">CONCENTRATION</p>
              <div class="w-line"></div>
              <div class="con_item_left_font mt-28">我们只专注于网站建设，客户的成功是我们大的荣耀</div>
            </div>
          </div>
           <div class="desc_con_item flex-x-between">
            <div class="con_item_left">
              <p>品牌领航</p>
              <p class="my-12">BRAND PIONEER</p>
              <div class="w-line mb-20"></div>
              <div class="con_item_left_font mt-28">上千家公司网站设计制作的选择，客户的成功是我们大的荣耀</div>
            </div>
          </div>
           <div class="desc_con_item d_flex">
            <div class="con_item_left">
              <p>专业品质</p>
              <p class="my-12">PROFESSIONAL QUALITY</p>
              <div class="w-line mb-20"></div>
              <div class="con_item_left_font mt-28">我们追求网站的制作质量，客户的成功是我们大的荣耀</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="banner_box">
      <el-carousel :interval="5000" arrow="always">
        <el-carousel-item v-for="item in 2" :key="item">
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
        </el-carousel-item>
      </el-carousel>
    </div>
    <div class="information">
      <div class="info_con">
        <div class="info_top">
          <p class="text-16">新闻资讯—新动态一手掌握</p>
          <div class="d-flex text-48">INFORMATION <p class="smBox"></p></div>
        </div>
        <div class="info_bottom flex-x-between mt-20">
          <div class="info_bottom_left">
            <div></div>
          </div>
          <div class="ml-32 info_bottom_right">
            <div class="mb-12">
              <h3>网站打开速度对网站自然排名的影响以及怎么解决</h3>
              <p class="mt-12">影响搜索引擎的排名细节因素有很多，每个细节都做到位了，网站自然排名才有可能提升。客户体验是每个搜索引擎都非常重视的，如果一个网站，打开速度很慢，甚至打开速度按秒来计算，别说搜索引擎，就算企业网站管理人员自己也会感觉很不合理。怎么样让打开速度更快，至少在用户和搜索引擎都接受的范围内打开，就显示得尤为重要了。</p>
              <p class="my-12">2021-03-16</p>
            </div>
            <div class="mb-12">
              <h3>网站打开速度对网站自然排名的影响以及怎么解决</h3>
              <p class="mt-12">影响搜索引擎的排名细节因素有很多，每个细节都做到位了，网站自然排名才有可能提升。客户体验是每个搜索引擎都非常重视的，如果一个网站，打开速度很慢，甚至打开速度按秒来计算，别说搜索引擎，就算企业网站管理人员自己也会感觉很不合理。怎么样让打开速度更快，至少在用户和搜索引擎都接受的范围内打开，就显示得尤为重要了。</p>
              <p class="my-12">2021-03-16</p>
            </div>
             <div class="mb-12">
              <h3>网站打开速度对网站自然排名的影响以及怎么解决</h3>
              <p class="mt-12">影响搜索引擎的排名细节因素有很多，每个细节都做到位了，网站自然排名才有可能提升。客户体验是每个搜索引擎都非常重视的，如果一个网站，打开速度很慢，甚至打开速度按秒来计算，别说搜索引擎，就算企业网站管理人员自己也会感觉很不合理。怎么样让打开速度更快，至少在用户和搜索引擎都接受的范围内打开，就显示得尤为重要了。</p>
              <p class="my-12">2021-03-16</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "../components/header.vue"
// import Footer from "../components/footer.vue";
export default {
    name: "Home",
    // components: { Footer },
    data() {
        return {};
    },
    methods: {
        handleSelect(val) {
            console.log("val", val);
        }
    },
    components: { Header }
}
</script>
<style lang="scss" scoped>
@import './home'

</style>