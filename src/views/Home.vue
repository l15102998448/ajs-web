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
              <el-row>
                <div>
                  <h5 class="text-18 mb-12">网站优化之常见问题的一些问题</h5>
                  <p class="text-14">网站是企业对外展示信息的重要方式之一，因此，很多企业都搭建了自己的网站，但是，要想发挥网站应有的作用，企业还需要对网站进行推广……</p>
                  <span><i class="el-icon-right"></i> 查看详情</span>
                </div> 

              </el-row>
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
    <div class="contact-box">
      <div class="contact-sub-box">
        <el-row :gutter="20">
          <el-col :span="16">
              <ul class="grid-content_01 text-14 ml-160 mb-48">
                <li>
                  <i class="el-icon-location-information text-16 mr-8"></i>
                  <span style="white-space:pre">地址：中国北京市东城区某某大厦8-88室</span>
                </li>
                 <li>
                  <i class="el-icon-phone-outline text-16 mr-8"></i>
                  <span style="white-space:pre">电话：400xxx8888</span>
                </li>
                 <li>
                  <i class="el-icon-printer text-16 mr-8"></i>
                  <span style="white-space:pre">传真：010xxxx88888</span>
                </li>
                 <li>
                  <i class="el-icon-message text-16 mr-8"></i>
                  <span style="white-space:pre">邮箱：name@example.xxx</span>
                </li>
              </ul>
              <div class="flex-x-start ml-160">
                <el-button round>更多联系信息</el-button>
              </div>
          </el-col>
          <el-col :span="8">
            <div class="grid-content_02">
              <div>您的需求是我们</div>
              <div class="d-flex">合作的开始 <p class="smBox"></p></div>
              <p class="text-24 mt-40">我们时刻期待着与您的沟通</p>
              <p class="mt-12">We look forward to communicating with you all the time</p>
            </div>
            </el-col>
        </el-row>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/header.vue"
import Footer from "../components/footer.vue";
export default {
    name: "Home",
    components: { Header, Footer },
    data() {
        return {};
    },
    methods: {
        handleSelect(val) {
            console.log("val", val);
        }
    },
}
</script>
<style lang="scss" scoped>
@import './home'

</style>