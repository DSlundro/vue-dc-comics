<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <NavCards />
    <SiteFooter />
  </div>
</template>

<script>
import SiteMain from "@/components/MainComponent.vue";
import SiteHeader from "@/components/HeaderComponent.vue";
import SiteFooter from "@/components/FooterComponent.vue";
import NavCards from "@/components/NavCardsComponent.vue";

export default {
  name: 'App',
  components: {
    SiteMain,
    SiteHeader,
    SiteFooter,
    NavCards,
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
</style>
