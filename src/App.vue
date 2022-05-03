<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <SiteFooter />
  </div>
</template>

<script>
import SiteMain from "@/components/MainComponent.vue";
import SiteHeader from "@/components/HeaderComponent.vue";
import SiteFooter from "@/components/FooterComponent.vue";

export default {
  name: 'App',
  components: {
    SiteMain,
    SiteHeader,
    SiteFooter,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
