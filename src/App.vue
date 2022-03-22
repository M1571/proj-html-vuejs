// ------------------------------------
// HTML

<template>

  <div id="app">
  <!-- <Nome /> -->
    <Header />
    <Section1 />
  </div>

</template>

// ------------------------------------
// JS

<script>

// import Nome from 'percorso file'
import Header from './components/HeaderMain.vue'
import Section1 from './components/FirstSection.vue'

export default {
  name: 'App',
  components: {
    // Nome,
    Header,
    Section1,
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
