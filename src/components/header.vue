<!-- 头部组建 -->
<template>
    <div :class="[ hasBg?'top-header':'']">
        <div class="home_top flex-x-between flex-y-center">
            <img src="../assets/images/logo.png"/>
            <el-menu :default-active="activeIndex"
                class="el-menu-demo"
                mode="horizontal"
                text-color="#fff"
                active-text-color="#ff5c35"
                @select="handleSelect">
                <el-menu-item v-for="(item,index) in titleList" :index="item.index" :key="index">{{item.label}}</el-menu-item>
            </el-menu>
        </div>
    </div>

</template>

<script>
export default {
    props: {
        activeIndex: {
            type: String,
            default: '/home'
        },
        hasBg: {
            type: Boolean,
            default: false
        }
    },
    data() {
        return {
            // activeIndex:"/home",
            titleList: [
                { index:'/home', label: '首页',path: '/home'},
                { index:'/about', label: '关于我们', path: '/about'},
                { index:'/case', label: '客户案例', path: '/case'},
                { index:'/news', label: '新闻资讯', path: '/news'},
                // { index:'/service', label: '我们的服务', path: '/service'},
                { index:'/contact', label: '联系我们', path: '/contact'},


            ]
            // titleList: {
            //     "1":{ label: '首页',path: '/home'},
            //     "2":{ label: '关于我们', path: '/about'},
            //     "3":{ label: '客户案例', path: '/case'},
            //     "4":{ label: '新闻资讯', path: '/news'},
            //     "5":{ label: '我们的服务', path: '/service'},
            //     "6":{ label: '联系我们', path: '/contact'},

            // }
        }
    },
    //生命周期 - 创建完成（访问当前this实例）
    created() {

    },
    //生命周期 - 挂载完成（访问DOM元素）
    mounted() {

    },
    methods: {
        handleSelect(indexPath){
            this.$router.push({ path: indexPath })
        }
    }
}
</script>
<style lang="scss" scoped>
/* @import url(); 引入css类 */
.top-header{
    background: rgb(34, 34, 34);
}
.home_top{
    width:80%;
    margin: 0 auto;
    height: 70px;

    img{
        width: 95px;
        height: 35px;
    }
    .el-menu.el-menu--horizontal{
      border: none;
      background: none;
    }
    .el-menu-item {
      transition: none;
      margin-left: 20px !important;
    }
    .el-menu-item:focus, .el-menu-item:hover,.el-menu-item.is-active{
       background: none !important;
       border: none !important;
    }
}
</style>
