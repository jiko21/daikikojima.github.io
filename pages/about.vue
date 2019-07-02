<template>
  <div class="container">
    <div>
      <h1 class="title">
        about me...
      </h1>
      <terminal-box>
        <p>$ show Career</p>
        <ul>
          <li>2014.4 ~ 2018.3: Kyoto Univ, Fac of Engineering, Dept of Informatics</li>
          <li>2017.4 ~ 2018.3: Studied @ Information System Group</li>
          <li>2019.4 ~ Now: Kyoto Univ, Grad School of Informatics, Dept of System Science</li>
          <li>2019.4 ~ Now: Studying @ Nakashima lab (Applied Informatics Group)</li>
        </ul>
      </terminal-box>
      <terminal-box>
        <p>$ show Skill</p>
        <ul>
          <li>C/C++</li>
          <li>JavaScript/TypeScript</li>
          <ul>
            <li>Node.js</li>
            <li>Vue.js (Vuex)</li>
            <li>React</li>
          </ul>
          <li>Java/Kotlin</li>
          <ul>
            <li>Android apps</li>
            <li>Spring boot (a little bit)</li>
          </ul>
          <li>Swift (iOS dev)</li>
          <li>Ruby (on Rails)</li>
          <li>Python</li>
          <ul>
            <li>Data visualization</li>
            <li>Web scraping</li>
            <li>Web (Django)</li>
          </ul>
        </ul>
      </terminal-box>
    </div>
  </div>
</template>

<script>
import TerminalBox from '~/components/TerminalBox.vue'

export default {
  components: {
    TerminalBox
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
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }

  li {
    list-style: none;
    margin: 2% 0;
  }
</style>
