<template>
  <div id="app">
    <HeaderDc />
    <MainCenter />
    <SecondContent />
    <FooterMain />
    <FooterSocial />

  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue';
import MainCenter from './components/MainCenter.vue';
import SecondContent from './components/SecondContent.vue';
import FooterMain from './components/FooterMain.vue';
import FooterSocial from './components/FooterSocial.vue';

export default {
  name: 'App',
  components: {
    HeaderDc,
    MainCenter,
    SecondContent,
    FooterMain,
    FooterSocial,
  }
}
</script>

<style lang="scss">
@import './assets/style/style.scss';
#app{
  font-family: 'Raleway', sans-serif;
}
</style>
