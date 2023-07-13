<script>
import HeaderNav from "./components/HeaderNav.vue"
import MainComponent from "./components/MainComponent.vue"

export default {
  name: 'App',
  components: {
    HeaderNav,
    MainComponent
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

  <footer>
    FOOTER
  </footer>

</template>

<style lang="scss">
  @use "./assets/scss/main.scss"
</style>
