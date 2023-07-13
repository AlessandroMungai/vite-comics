<script>
import HeaderNav from "./components/HeaderNav.vue"

export default {
  name: 'App',
  components: {
    HeaderNav
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

  <main>
    MAIN
  </main>

  <footer>
    FOOTER
  </footer>

</template>

<style lang="scss">
  @use "./assets/scss/main.scss"
</style>
