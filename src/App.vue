<template>
  <Navbar/>
  <router-view/>
  <About/>
  <Auction/>
  <Footer/>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import About from '@/views/About.vue'
import Auction from '@/views/Trending.vue'


export default {
  components: {
    Navbar,
    About,
    Auction,
    Footer
  }
}
</script>

<style lang="scss" scoped>
#app {
  font-family: $font-family;
  min-height: 100vh;
}

</style>
