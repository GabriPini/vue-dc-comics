<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <SiteBanner />
    <SiteFooter />
  </div>
</template>

<script>
import SiteHeader from '@/components/headerComponent.vue';
import SiteMain from '@/components/mainComponent.vue'
import SiteFooter from './components/footerComponent.vue'
import SiteBanner from './components/bannerComponent.vue'
export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteBanner,
    SiteFooter,
  }
}
</script>

<style lang="scss">
@import './style/general.scss';
@import './style/variables.scss';
</style>