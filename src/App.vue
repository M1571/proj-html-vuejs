// ------------------------------------
// HTML

<template>

  <div id="app">
  <!-- <Nome /> -->
    <Header />
    <Section1 />
    <Section2 />
    <Section5 />
    <Footer />
  </div>

</template>

// ------------------------------------
// JS

<script>

// import Nome from 'percorso file'
import Header from './components/HeaderMain.vue'
import Section1 from './components/FirstSection.vue'
import Section2 from './components/SecondSection.vue'
import Section5 from './components/FifthSection.vue'
import Footer from './components/FooterMain.vue'

export default {
  name: 'App',
  components: {
    // Nome,
    Header,
    Section1,
    Section2,
    Section5,
    Footer,
  }
}
</script>

// ------------------------------------
// CSS

<style lang="scss">

// @import 'percorso file';
@import './assets/scss/_mixins.scss';
@import './assets/scss/_varcolori.scss';

// ------------------------------------
// CSS COMMON

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  @include container;
} 

img {
  max-width: 100%;
}

a {
  text-decoration: none; 
  color: currentColor;
}

ol, ul {
  list-style: none;
}

// ------------------------------------

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
  font-weight: 700;
}

</style>

// ------------------------------------
