<template>
  <div class="container">
    <div>
      <h1 class="title">
        Works
      </h1>
      <Apps/>
    </div>
    <p>Google Play and the Google Play logo are trademarks of Google LLC.</p>
  </div>
</template>

<script>
  import Apps from '~/components/Apps.vue'
  import CharToHeader from '~/static/charto_header.png'

  export default {
    components: {
      Apps,
    },
    data() {
      return {
        charto_header: CharToHeader,
      }
    }
  }
</script>

<style lang="scss" scoped>
  .container {
    margin: 0 auto;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 50px;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 30px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }
</style>
