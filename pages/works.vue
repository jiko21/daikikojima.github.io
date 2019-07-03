<template>
  <div class="container">
    <div>
      <h1 class="title">
        Works
      </h1>
      <div id="apps">
        <h2 class="subtitle">App</h2>

      </div>
    </div>
  </div>
</template>

<script>
  import SocialIcon from '~/components/SocialIcon.vue'
  import GitHubImage from '~/static/github.png'
  import TwitterImage from '~/static/twitter.png'
  import SlidesImage from '~/static/slides.svg'
  export default {
    components: {
      SocialIcon
    },
    data() {
      return {
        github_img: GitHubImage,
        twitter_img: TwitterImage,
        slides_img: SlidesImage
      }
    }
  }
</script>

<style>
  .container {
    margin: 0 auto;
    display: flex;
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
