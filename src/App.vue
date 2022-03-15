<template>
  <Navbar/>
  <router-view/>
  <Footer/>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
export default {
  components: {
    Navbar,
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
