<script>
import HeaderNav from "./components/HeaderNav.vue"
import MainComponent from "./components/MainComponent.vue"
import SecondSection from "./components/SecondSection.vue"
import FooterNav from "./components/FooterNav.vue"

export default {
  name: 'App',
  components: {
    HeaderNav,
    MainComponent,
    SecondSection,
    FooterNav
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

</template>

<style lang="scss">
  @use "./assets/scss/main.scss"
</style>
