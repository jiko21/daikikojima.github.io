<template>
  <div class="info-boxes">
    <terminal-box>
      <p>$ show Career</p>
      <ul class="terminal-rst">
        <li>2014.4 ~ 2018.3: Kyoto Univ, Fac of Engineering, Dept of Informatics</li>
        <li>2017.4 ~ 2018.3: Studied @ Information System Group</li>
        <li>2019.4 ~ Now: Kyoto Univ, Grad School of Informatics, Dept of System Science</li>
        <li>2019.4 ~ Now: Studying @ Nakashima lab (Applied Informatics Group)</li>
      </ul>
    </terminal-box>
    <terminal-box>
      <p>$ show Skill</p>
      <ul class="terminal-rst">
        <li>C/C++</li>
        <li>JavaScript/TypeScript (especially skillful)</li>
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
        <li>Swift</li>
        <ul>
          <li>iOS App Develop</li>
        </ul>
        <li>Ruby</li>
        <ul>
          <li>Ruby on Rails</li>
        </ul>
        <li>Python</li>
        <ul>
          <li>Data visualization</li>
          <li>Web scraping</li>
          <li>Web (Django)</li>
        </ul>
      </ul>
    </terminal-box>
  </div>
</template>

<script>
  import TerminalBox from '~/components/TerminalBox.vue'
  export default {
    name: "InfoBoxes",
    components: {
      TerminalBox
    }
  }
</script>

<style lang="scss" scoped>
  ul{
    &.terminal-rst{
      padding: 0;
    }
    li {
      list-style: none;
      margin: 2% 0;
    }
  }
  .terminal-img {
    height: 100px;
  }
</style>