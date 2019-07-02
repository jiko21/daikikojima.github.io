<template>
  <div class="container">
    <div>
      <img id="my-img" src="~/static/profile.jpg"/>
      <h1 class="title">
        Daikids
      </h1>
      <h2 class="subtitle">
        (un) official site
      </h2>
      <div class="social">
        <SocialIcon
          :title='"GitHub"'
          :url='"https://github.com/daikikojima"'
          :img="github_img"
          color="#333"
        />
        <SocialIcon
          :title='"Twitter"'
          :url='"https://twitter.com/Daikids2"'
          :img="twitter_img"
          color="#55acee"
        />
        <SocialIcon
          :title='"My Slides"'
          :url='"https://speakerdeck.com/daikids2"'
          :img="slides_img"
          color="#ccc"
        />
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
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  #my-img {
    height: 400px;
    margin: auto;
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

  .social {
    margin: auto;
    display: flex;
    width: 300px;
  }

</style>
