<template>
  <Navbar/>
  <router-view/>
  <About/>
  <Auction/>
  <Creators/>
  <Footer/>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import About from '@/views/About.vue'
import Auction from '@/views/Trending.vue'
import Creators from '@/views/Creators.vue'


export default {
  components: {
    Navbar,
    About,
    Auction,
    Creators,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  min-height: 100vh;
  font-family: $font-family;
}

</style>
