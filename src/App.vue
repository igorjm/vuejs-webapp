<template>
  <div class="main">
    <header-main-page />
    <home-section />
    <about-section />
    <campanhas-section />
    <footer-main-page />
  </div>
</template>

<script>
import HeaderMainPage from './components/Headers/Header';
import FooterMainPage from './components/Footer/Footer';
import Home from './components/Home/Home';
import About from './components/About/About'
import Campanhas from './components/Campanhas/Campanhas'

export default {
  name: 'App',
  components: {
    'header-main-page': HeaderMainPage,
    'footer-main-page': FooterMainPage,
    'home-section': Home,
    'about-section': About,
    'campanhas-section': Campanhas
  }
}
</script>

<style>

.main {
  font-family: "Myriad Pro", "Gill Sans", "Gill Sans MT", Calibri, sans-serif;
  font-weight: 400;
  width: 1920px;
  height: 100px;
}

*, *:before, *:after {
  box-sizing: inherit;
}

a {
  text-decoration: none;
}

</style>