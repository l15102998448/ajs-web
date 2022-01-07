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

        <div class="question-box p-80">
            <div class="question-container">
                <ul class="flex-x-around flex-wrap">
                    <li v-for="item in 6" :key="item">
                        <p class="w-al-date text-14">2021-03-16</p>
                        <h5 class="w-al-title pt-24">网站空间应该怎么选择？</h5>
                        <p class="w-al-desc pt-24 text-12">网站上线必须用到服务器，或者虚拟空间。无论是虚拟空间或者服务器（以下我们就都称为网站空间）是用来放置网页代码程序和数据资料的地方。是个虚拟的东西。</p>
                        <p class="w-al-btn pt-48 text-12">查看详情 &gt; </p>
                    </li>
                </ul>
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
.news-page{
    .news-bg-style{
        background-image: url("../assets/images/news-bg.jpeg");
        background-position: 0% 50%;
        background-size: cover;
    }
    .el-divider{
        position: absolute;
        top: 69px;
        background: #d1d6d96e;
        margin: 0;
    }
    .news-container{
        width: 80%;
        margin: 0 auto;
        position: relative;
        min-height: 429px;
        .editableContent{
            font-family:Verdana,Geneva,sans-serif;
            text-align: left;
            h1{
                color:#ffffff;
                font-size: 46px;
                font-weight: bold;
                line-height: 80px;
                span{
                    color: #ff5c35;
                }
            }
            p{
                color:#bbbbbb;
                b{
                    border-left-width: 3px;
                    border-left-style: solid;
                    border-left-color: #ff5c35;
                }
            }
        }
    }
    .question-box{
        background: #ffffff;
        .question-container {
            /*width: 80%;*/
            margin: 0 auto;
            min-height: 600px;
            ul > li{
                box-sizing: border-box;
                padding: 56px 30px 0;
                width: 380px;
                height: 310px;
                min-width: 100px;
                margin: 0 0 30px 30px;
                overflow: hidden;
                float: left;
                list-style: none;
                cursor: pointer;
                background-color: #FFFFFF;
                text-align: left;
                box-shadow: 0 5px 30px 0 #0000001a;
                .w-al-date{
                    color: #989898;
                    font-weight: bold;
                    font-style: normal;
                    font-family: Tahoma;
                    line-height: 20px;
                    overflow: hidden;
                    text-overflow: ellipsis;
                    white-space: nowrap;
                }
                h5{
                    font-size: 18px;
                    color: #262626;
                    font-weight: bold;
                    font-style: normal;
                    text-decoration: none;
                    font-family: 'Noto Sans CJK';
                    line-height: 22px;
                    display: -webkit-box;
                    -webkit-box-orient: vertical;
                    -webkit-line-clamp: 1;
                    overflow: hidden;
                }
                .w-al-desc {
                    color: #989898;
                    font-weight: normal;
                    height: calc(22px * 2);
                    line-height: 22px;
                    display: -webkit-box;
                    -webkit-box-orient: vertical;
                    -webkit-line-clamp: 2;
                    overflow: hidden;
                }
                .w-al-btn{

                    color: #5f467b;
                    font-weight: bold;
                    font-style: normal;
                    text-decoration: none;
                    font-family: 'Noto Sans CJK';
                    line-height: 17px;
                    overflow: hidden;
                    text-overflow: ellipsis;
                    white-space: nowrap;
                }
            }
        }
    }
}
</style>
