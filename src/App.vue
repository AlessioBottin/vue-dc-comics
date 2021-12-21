<template>
  <div id="app">
    <Header />
    
    <main>
      <Banner />

      <ComicsList />
    </main>

    <PreFooter />

    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Banner from "./components/Banner.vue";
import ComicsList from "./components/ComicsList.vue";
import PreFooter from "./components/PreFooter.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Banner,
    ComicsList,
    PreFooter,
    Footer,
  },
};
</script>

<style lang="scss">
@import './style/general';
@import './style/utilities';
@import './style/variables';

</style>
