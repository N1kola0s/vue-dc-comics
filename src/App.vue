<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <SiteFooter />
  </div>
</template>

<script>

/* importo come componente l'Header del sito */
import SiteHeader from "@/components/HeaderComponent.vue";

/* importo come componente il Main del sito */
import SiteMain from "@/components/MainComponent.vue";

/* importo come componente il Footer del sito*/
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
/* importo lo stile */
  @import '@/assets/scss/style';

</style>
