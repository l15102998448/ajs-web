<!-- 新闻资讯 -->
<template>
    <div class="news-page">
        <div class="news-bg-style">
            <Header activeIndex="/news"/>
            <el-divider />
            <div class="news-container flex-y-center">
                <el-row class="editableContent mb-40">
                    <h1><span>I</span>NFORMATION</h1>
                    <p class="text-14"><b class="mr-20"></b>新闻资讯—客户的成功是我们大的荣耀</p>
                </el-row>
            </div>
        </div>

        <div v-if="!showDetails" class="question-box p-80">
            <div class="question-container">
                <ul class="flex-x-around flex-wrap">
                    <li v-for="(item,index) in questionList" :key="index">
                        <p class="w-al-date text-14">{{item.time}}</p>
                        <h5 class="w-al-title pt-24">{{item.title}}</h5>
                        <p class="w-al-desc pt-24 text-12">{{item.desc}}</p>
                        <p class="w-al-btn pt-48 text-12" @click="showDetails = true">查看详情 &gt; </p>
                    </li>
                </ul>
            </div>
        </div>
        <div v-else class="question-list">
            <div class="quest-con">
                <h1 class="w-title text-24">网站空间应该怎么选择？</h1>
                <div class="quest-desc text-14 my-40">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网站上线必须用到服务器，或者虚拟空间。无论是虚拟空间或者服务器（以下我们就都称为网站空间）是用来放置网页代码程序和数据资料的地方。是个虚拟的东西。在选择购买的时候很多用户都不知道，需要怎么购买，购买什么样的？多大的空间？这些都是需要根据网站具体使用情况作为依据。下面我们就根据自身经验为大家介绍一下，选择什么样的空间？应该从哪几方面去选择？</div>
                <h3><span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;一：选择知名服务商</span></h3>
                <div class="quest-desc text-14 my-20">
                    <span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;现在，网络社会发展的迅速，各种网站公司层出不穷，域名空间服务商也是多如牛毛。价格也是差别很大，我们建议选择一些被大众认可的服务商。像阿里云（原万网）、西部数码、新网、腾讯云和百度云（这是近几年才发展的），这些大的服务商经济实力雄厚，有自己专业的业务技术团队，出现问题不会出现找不到人解决处理的问题。</span>
                </div>
                <h3><span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;二：根据网站程序开发环境</span></h3>
                <div class="quest-desc text-14 my-20">
                    <span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网站开发程序语言分ASP/PHP/JSP/.NET这四种，网站空间分windows系统和linux系统，无论哪种系统在购买的时候你看下，只要支持你的网站程序就可以（好选择windows系统，这样以后上传管理也方便）。</span>
                </div>
                <h3><span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;三：网站所需要使用的空间大小</span></h3>
                <div class="quest-desc text-14 my-20">
                    <span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      网站程序代码一般从几M到几十M都不等，这个不是主要的问题，因为现在空间小的都是以G为单位的，所以，你需要考虑的大小是以后上传的网站资料内容有多大。比方说要考虑要上传多少张图片，每张图片大概多大，网页图片用到的都是200K以内，如果你的图片都是自己拍照或者都是几M的，建议用做图软件处理小一点。网站上有没有视频什么的，总体就以下几种。</span>
                    <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;（1）图片大小*图片张数，来计算图片大概用多大空间；</p>
                    <p class="my-8">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;（2）有没有视频，根据视频多少和大小来计算；</p>
                    <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;（3）有没有下载压缩包或其它文档；</p>
                   
                    <p class="mt-12">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;根据上面几点来综合考虑用多大的空间合适，一般不用考虑几年以后的事，因为网站如果不够了，可以升级，你只要保证近期够用即可。</p>
                </div>
                 <h3><span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;四：网站访问量（重要）</span></h3>
                <div class="quest-desc text-14 my-20">
                    <span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;            因为现在网站空间都有月流量限制。费用越贵购买到的空间越大，流量越多。一般企业网站如果不做推广月20G流量就够用，如果做推广那60G以上的流量才可以。这个在以后使用的过程中也可以根据访问统计报告来看下具体每个月用多少。</span>
                </div>
                <div class="quest-desc text-14 my-20">
                    <span >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;            购买空间适合自己就行，因为每年都要续费，购买大的费用贵，如果用不上就浪费了。还有个，在选择服务商时，虽然，每家服务商在网上都有负面信息，但也不能全信，毕竟只有购买使用的人多，出现问题的几率才越大。</span>
                </div>
                      
            </div>
        </div>
        <Footer />
    </div>
</template>

<script>
import Header from "../components/header.vue"
import Footer from "../components/footer.vue";
export default {
    data() {
        return {
            showDetails: false,
            questionList: [
                { 
                    time: '2021-11-12',
                    title: '网站空间应该怎么选择？',
                    desc: '网站上线必须用到服务器，或者虚拟空间。无论是虚拟空间或者服务器（以下我们就都称为网站空间）是用来放置网页代码程序和数据资料的地方。是个虚拟的东西。',
                },
                { 
                    time: '2021-11-12',
                    title: '网站优化之常见问题的一些问题',
                    desc: '网站是企业对外展示信息的重要方式之一，因此，很多企业都搭建了自己的网站，但是，要想发挥网站应有的作用，企业还需要对网站进行推广，让网站可以快速进入人们的视线，从而获得更多客户资源。推广分两种方式，一种是花钱做竞价排名，另一种是优化。',
                },
                { 
                    time: '2021-11-12',
                    title: '网站打开速度对网站自然排名的影响以及怎么解决',
                    desc: '影响搜索引擎的排名细节因素有很多，每个细节都做到位了，网站自然排名才有可能提升。客户体验是每个搜索引擎都非常重视的，如果一个网站，打开速度很慢，甚至打开速度按秒来计算，别说搜索引擎，就算企业网站管理人员自己也会感觉很不合理。怎么样让打开速度更快，至少在用户和搜索引擎都接受的范围内打开，就显示得尤为重要了。',
                },
                { 
                    time: '2021-11-12',
                    title: '用户喜欢什么样的网站设计',
                    desc: '网站想要被用户所喜欢，企业在设计网站时就要迎合用户喜好。对于一些中小企业，他们关心的不是功能，而是设计效果能不能完美的体现出自己的文化内涵，否吸引顾客，让客户好快速的了解自己，信任自己。',
                },
                { 
                    time: '2021-11-12',
                    title: '网站空间应该怎么选择？',
                    desc: '网站上线必须用到服务器，或者虚拟空间。无论是虚拟空间或者服务器（以下我们就都称为网站空间）是用来放置网页代码程序和数据资料的地方。是个虚拟的东西。',
                },
                { 
                    time: '2021-11-12',
                    title: '网站优化之常见问题的一些问题',
                    desc: '网站是企业对外展示信息的重要方式之一，因此，很多企业都搭建了自己的网站，但是，要想发挥网站应有的作用，企业还需要对网站进行推广，让网站可以快速进入人们的视线，从而获得更多客户资源。推广分两种方式，一种是花钱做竞价排名，另一种是优化。',
                }
            ]
        };
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
@import "../views/otherFile/news";
</style>
