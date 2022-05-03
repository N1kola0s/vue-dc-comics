<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <SiteFooter />
  </div>
</template>

<script>
/* import HelloWorld from './components/HelloWorld.vue' */
import SiteHeader from "@/components/HeaderComponent.vue";
import SiteMain from "@/components/MainComponent.vue";
import SiteFooter from "@/components/FooterComponent.vue";


export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
    /* HelloWorld */
  }
}
</script>

<style lang="scss">
  @import '@/assets/scss/style';

</style>
