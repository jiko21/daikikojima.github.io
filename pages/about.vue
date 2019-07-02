<template>
  <div class="container">
    <div>
      <h1 class="title">
        about me...
      </h1>
      <section class="section-box">
        <h2>Career</h2>
        <ul>
          <li class="font-sans text-lg">2014.4 ~ 2018.3: Kyoto Univ, Fac of Engineering, Dept of Informatics And Applud Math & Physics</li>
          <li class="font-sans text-lg">2017.4 ~ 2018.3: Studied @ Information System Group</li>
          <li class="font-sans text-lg">2019.4 ~ Now: Kyoto Univ, Grad School of Informatics, Dept of System Science</li>
          <li class="font-sans text-lg">2019.4 ~ Now: Studying @ Nakashima lab (Applied Informatics Group)</li>
        </ul>
      </section>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
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
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.section-box {
  width: 100%;
  background: #00C48D;

}
</style>
