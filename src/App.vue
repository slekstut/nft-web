<template>
  <Navbar/>
  <router-view/>
  <About/>
  <Footer/>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import About from '@/views/About.vue'


export default {
  components: {
    Navbar,
    About,
    Footer
  }
}
</script>

<style lang="scss">
body {
  background-color: $color-sand;

}
#app {
  min-height: 100vh;
  font-family: $font-family;
}

</style>
