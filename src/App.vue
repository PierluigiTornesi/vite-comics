<script>
  
  import AppHeader from './components/AppHeader.vue';
  import ProductList from './components/ProductList.vue';
  import AppIcons from './components/AppIcons.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppBanner from './components/AppBanner.vue';

  export default{
    components:{
    AppHeader,
    ProductList,
    AppFooter,
    AppIcons,
    AppBanner,
    }
  }
</script>

<template>
  <AppHeader />
  <AppBanner />
  <ProductList />
  <AppIcons />
  <AppFooter />
</template>

<style lang="scss">
@use "./style/general.scss"
</style>
