<template>
  <div id="app">
    <Header />
    <Main />
    <BluePanel />
    <FooterTop />
    <FooterBottom />
  </div>
</template>

<script>
import Header from './components/header.vue'
import Main from './components/main.vue'
import BluePanel from './components/blue-panel.vue'
import FooterTop from './components/footer-top.vue'
import FooterBottom from './components/footer-bottom.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    BluePanel,
    FooterTop,
    FooterBottom
  }
}
</script> 

<style lang="scss">
@import "./style/variables.scss";
@import "./style/general-rules.scss";

#app {
  font-family: '$primaryFont', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>