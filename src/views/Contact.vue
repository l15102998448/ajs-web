<!-- 联系我们 -->
<template>
    <div class="contact-page">
        <div class="contact-bg-style">
            <Header activeIndex="/contact"/>

            <el-divider />
            <div class="contact-container flex-y-center">
                <el-row class="editableContent mb-40">
                    <h1><span>C</span>ONTACT US</h1>
                    <p class="text-14"><b class="mr-20"></b>联系我们—客户的成功是我们大的荣耀</p>
                </el-row>
            </div>
        </div>
        <div class="contact-box py-80">
            <div class="flex-x-between" style="width: 80%;margin: auto">
                <div class="contact-left">
                    <h1>您的需求是我们合作的开始</h1>
                    <h4 class="text-14">我们时刻期待着与您的沟通</h4>
                    <ul class="grid-content_01 text-14 mt-40 mb-48">
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
                </div>
                <div class="contact-right">
                    <h1 class="text-20">关注我们<span class="text-14 ml-12">FOLLOW US</span></h1>
                    <div class="contact-ways p-12 mt-16">
                        <p class="smBox"></p>
                        <el-row class="flex-x-between">
                            <el-col :span="12" class="flex-center flex-column">
                                <img src="../assets/images/contact-01.png" alt="">
                                <p class="text-14 mt-12">微信公众号</p>
                            </el-col>
                            <el-col :span="12" class="flex-center flex-column">
                                <img src="../assets/images/contact-01.png" alt="">
                                <p class="text-14 mt-12">微信公众号</p>
                            </el-col>
                        </el-row>
                        <div class="flex-x-end">
                            <p class="smBox "></p>
                        </div>
                    </div>
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
.contact-page {
    .contact-bg-style {
        background-image: url("../assets/images/contact-bg.jpeg");
        background-position: 0% 50%;
        background-size: cover;
    }

    .el-divider {
        position: absolute;
        top: 69px;
        background: #d1d6d96e;
        margin: 0;
    }
    .contact-container{
        min-height: 429px;
        .editableContent{
            width: 80%;
            margin: auto;
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
    .contact-box{
        background: #ffffff;
        /*min-height: 500px;*/
        .contact-left{
            text-align: left;
            h1{
                line-height:1.5;
                color:#ff5c35;
                font-family:Microsoft JhengHei;
                font-size:30px;
                font-weight: bold;
            }
            h4{
                font-family:Source Han Sans;
            }
        }
        .grid-content_01{
            color: #666;
            text-align: left;
            li{
                line-height: 2;
                i{
                    color: #ff5c35;
                }
            }
        }
        .contact-right{
            h1{
                color:#333333;
                font-weight: bold;
                text-align: left;
                span{
                    color: #ff5c35;
                    letter-spacing: 3px;
                    font-weight: normal;
                }
            }
            .contact-ways{
                width: 260px;
                background: rgb(237, 237, 244);
                img{
                    width: 87px;
                    height: 87px;
                }
            }
        }

    }
}
</style>
