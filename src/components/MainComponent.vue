<script>
export default {
  name: 'MainComponent',
  components: {

  },
  data(){
    return {
        title: 'Contents goes here'
    }
  },
  methods: {

  }
}
</script>

<template>

  <main>

    <div class="container">

        <h1>
            {{ title }}
        </h1>

    </div>

  </main>

</template>

<style scoped lang="scss">

    h1 {
        color:white;
        padding: 40px 0;
        font-size: 1.5rem;
    }

    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0;
    }

</style>