<template>
  <div class="about-box">
    <el-divider />
    <Header activeIndex="/about"/>
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
@import '../assets/styles/otherFile/about'

</style>