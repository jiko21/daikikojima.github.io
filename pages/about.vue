<template>
  <div class="container">
    <div>
      <h1 class="title">
        about me...
      </h1>
      <info-boxes/>
    </div>
  </div>
</template>

<script>
import InfoBoxes from '~/components/InfoBoxes.vue'

export default {
  components: {
    InfoBoxes
  }
}
</script>

<style lang="scss" scoped>
  .container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
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
</style>
