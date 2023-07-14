<script>
import HeaderNav from "./components/HeaderNav.vue"
import MainComponent from "./components/MainComponent.vue"
import SecondSection from "./components/SecondSection.vue"
import FooterNav from "./components/FooterNav.vue"
import FooterBottom from "./components/FooterBottom.vue"

export default {
  name: 'App',
  components: {
    HeaderNav,
    MainComponent,
    SecondSection,
    FooterNav,
    FooterBottom
  },
  data(){
    return {

    }
  },
  methods: {

  }
}
</script>

<template>

  <HeaderNav />

  <MainComponent />

  <SecondSection />

  <FooterNav />

  <FooterBottom />

</template>

<style lang="scss">
  @use "./assets/scss/main.scss"
</style>
