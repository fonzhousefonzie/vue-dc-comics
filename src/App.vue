<template>
  <div id="app">
    <TheHeader />
    <div class="section bg-dark text-light">
      <div class="container">
        <h4 class="text-start py-4 fw-bolder mb-0">--&gt; Contents goes here &lt;--</h4>
      </div>
    </div>
    <BannerBlue />
    <BannerCTA />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import BannerCTA from './components/BannerCTA.vue';
import BannerBlue from './components/BannerBlue.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    BannerCTA,
    BannerBlue
}
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

#app {
  font-family: 'Roboto Condensed', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

a{
  color: unset;
}
</style>
