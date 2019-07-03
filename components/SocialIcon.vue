<template>
  <div class="social-icon" :style="styles">         
    <a :title="title" :href="url" target="_blank">
      <img :src='img'/> 
    </a>  
  </div>
</template>
<script>
export default {
  name: 'SocialIcon',
  props: [
    'title',
    'url',
    'img',
    'color',
  ],
  computed: {
    // バインドするスタイルを生成
    styles () {
      return {
        '--color': this.color,
      }
    }
  }
}
</script>
<style lang="scss" scoped>
.social-icon {
  --color: red;
  background-color: var(--color);
  padding: 5px;
  width: 100%;
  margin: auto;
  &:hover {
    opacity: 0.6;
    transform: translateY(0.1em);
  }
}
img {
  width: 100%;
}
</style>
