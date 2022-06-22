<template>
  <div id="app">
    <TheHeader />
    <CardsBanner />
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
import CardsBanner from './components/CardsBanner.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    BannerCTA,
    BannerBlue,
    CardsBanner
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

button.primary{
  display: inline-block;
  background-color: #3f7ef8;
  font-size: 0.8rem;
  font-weight: bold;
  text-transform: uppercase;
  color: whitesmoke;
  border: none;
  padding: 0.5rem 3rem;

  &:hover{
    background-color: #588fff;
  }
}
</style>
