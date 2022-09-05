<template>
  <div id="app">
    <MainHeader/>
    <MainContent/>
    <ShopInfo/>
    <MainFooter/>
    <SocialFooter/>
  </div>
</template>

<script>
import MainHeader from '@/components/MainHeader.vue';
import MainContent from './components/MainContent.vue';
import ShopInfo from './components/ShopInfo.vue';
import MainFooter from './components/MainFooter.vue';
import SocialFooter from './components/SocialFooter.vue';



export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    ShopInfo,
    MainFooter,
    SocialFooter
}
}
</script>

<style lang="scss">

@import './style/index.scss';

</style>
