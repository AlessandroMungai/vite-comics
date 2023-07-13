<script>
import HeaderNav from "./components/HeaderNav.vue"
import MainComponent from "./components/MainComponent.vue"
import SecondSection from "./components/SecondSection.vue"

export default {
  name: 'App',
  components: {
    HeaderNav,
    MainComponent,
    SecondSection
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

  <footer>
    FOOTER
  </footer>

</template>

<style lang="scss">
  @use "./assets/scss/main.scss"
</style>
