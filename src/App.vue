<template>
  <div id="app">
    <Header />
    
    <main>
      <div class="container">
        content
      </div>
    </main>

    <InfoFooter />

    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import InfoFooter from "./components/InfoFooter.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    InfoFooter,
    Footer,
  },
};
</script>

<style lang="scss">
@import './style/general';
@import './style/utilities';
@import './style/variables';

main {
  background-color: #1c1c1c;
  height: 200px;
  color: white;
}
</style>
