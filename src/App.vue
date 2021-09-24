<template>
  <div id="app">
    <Header />
    <Main />
    <FooterTop />
    <FooterBottom />
  </div>
</template>

<script>
import Header from './components/header.vue'
import Main from './components/main.vue'
import FooterTop from './components/footer-top.vue'
import FooterBottom from './components/footer-bottom.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    FooterTop,
    FooterBottom
  }
}
</script> 

<style lang="scss">
@import "./style/variables.scss";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: '$primaryFont', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
