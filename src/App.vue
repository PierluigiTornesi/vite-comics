<script>
  
  import AppHeader from './components/AppHeader.vue';
  import ProductList from './components/ProductList.vue';
  import AppFooter from './components/AppFooter.vue';

  export default{
    components:{
    AppHeader,
    ProductList,
    AppFooter,
}
  }
</script>

<template>
  <h1>Titolo</h1>
  <AppHeader />
  <ProductList />
  <AppFooter />
</template>

<style lang="scss">
@use "./style/general.scss"
</style>
