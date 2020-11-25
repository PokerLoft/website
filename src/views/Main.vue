<template>
  <div>
      <Navbar/>
      <div class="background-second"></div>
      <div class="landing-pages">
        <LandingFirstPage/>
        <LandingSecondPage/>
        <LandingThirdPage/>
        <Footer/>
      </div>
  </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import LandingFirstPage from "../components/LandingFirstPage.vue";
import LandingSecondPage from "../components/LandingSecondPage.vue";
import LandingThirdPage from "../components/LandingThirdPage.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "Main",
  components: {
    Navbar,
    LandingFirstPage,
    LandingSecondPage,
    LandingThirdPage,
    Footer
  }
};
</script>

<style scoped>
.landing-pages {
    display: flex;
    flex-direction: column;
}

.background-second {
    position: absolute;
    width: 100%;
    height: 900px;
    margin: 1000px 0 0 0;
    background: rgba(231, 231, 231, 0.25);
    z-index: -1;
}
</style>
