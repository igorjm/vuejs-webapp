<template>
  <div class="main">
    <header-section />
    <home-section />
    <about-section />
    <campanhas-section />
    <saude-section />
    <onde-encontrar-section />
    <footer-section />
  </div>
</template>

<script>
import Vue from 'vue';
import BootstrapVue from 'bootstrap-vue';

import HeaderMainPage from './components/Headers/Header';
import FooterMainPage from './components/Footer/Footer';
import Home from './components/Home/Home';
import About from './components/About/About';
import Campanhas from './components/Campanhas/Campanhas';
import Saude from './components/Saude/Saude';
import OndeEncontrar from './components/OndeEncontrar/OndeEncontrar';

Vue.use(BootstrapVue);

export default {
  name: 'App',
  components: {
    'header-section': HeaderMainPage,
    'home-section': Home,
    'about-section': About,
    'campanhas-section': Campanhas,
    'saude-section': Saude,
    'onde-encontrar-section': OndeEncontrar,
    'footer-section': FooterMainPage,
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

</style>