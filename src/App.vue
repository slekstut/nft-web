<template>
  <navbar-component/>
  <router-view/>
  <about-component/>
  <trending-component/>
  <creators-component/>
  <contact-component/>
  <footer-component/>
</template>

<script>
import NavbarComponent from "@/components/NavbarComponent.vue";
import FooterComponent from "@/components/FooterComponent.vue";
import AboutComponent from '@/views/AboutComponent.vue'
import TrendingComponent from '@/views/TrendingComponent.vue'
import CreatorsComponent from '@/views/CreatorsComponent.vue'
import ContactComponent from '@/components/ContactComponent.vue'


export default {
  components: {
    NavbarComponent,
    AboutComponent,
    TrendingComponent,
    CreatorsComponent,
    ContactComponent,
    FooterComponent
  }
}
</script>

<style lang="scss">
#app {
  min-height: 100vh;
  font-family: $font-family;
}

</style>
