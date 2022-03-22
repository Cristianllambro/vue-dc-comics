<template>
  <div id="app">
    <HeaderDc />
    <MainCenter />
    <SecondContent />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue';
import MainCenter from './components/MainCenter.vue';
import SecondContent from './components/SecondContent.vue';

export default {
  name: 'App',
  components: {
    HeaderDc,
    MainCenter,
    SecondContent,
  }
}
</script>

<style lang="scss">
@import './assets/style/style.scss'
</style>
