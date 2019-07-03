<template>
  <div id="apps">
    <h2 class="subtitle">App</h2>
    <v-container grid-list-md text-xs-center>
      <v-layout row wrap>
        <v-flex xs6>
          <Card
            title="CharTo"
            :image="charto_header"
          >
            <p class="card-text">タスク管理ツールCharToです。
              ChartとTodoを掛け合わせたものとなっております。</p>
            <a
              target="_blank"
              href='https://play.google.com/store/apps/details?id=com.jikoapps.charto&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img
              alt='Get it on Google Play'
              src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png'
            /></a>
            <h3>使用技術</h3>
            <div class="techs">
              <div>
                <img src="~/static/kotlin_logo.png"/>
                <p>Kotlin</p>
              </div>
              <div>
                <img src="~/static/firebase_logo.png"/>
                <p>Firebase</p>
              </div>
            </div>
          </Card>
        </v-flex>
        <v-flex xs6>
          <Card
            title="MarkPark"
            :image="markpark_header"
          >
            <p class="card-text">自転車の駐輪場所を記録し、自転車探しを手助けするアプリです。</p>
            <a
              target="_blank"
              href='https://play.google.com/store/apps/details?id=com.jiko.bycicle&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img
              alt='Get it on Google Play'
              src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png'/></a>
            <h3>使用技術</h3>
            <div class="techs">
              <div>
                <img src="~/static/kotlin_logo.png"/>
                <p>Kotlin</p>
              </div>
              <div>
                <img src="~/static/map_icon.png"/>
                <p>Maps sdk for Android</p>
              </div>
            </div>
          </Card>
        </v-flex>
      </v-layout>
      <v-layout row wrap>
        <v-flex xs6>
          <Card
            title="CharTo for Web"
            :image="charto_web_header"
          >
            <p class="card-text">タスク管理ツールCharToのWeb版です。PWAにも対応しております。
              ChartとTodoを掛け合わせたものとなっております。</p>
            <a
              target="_blank"
              href='https://play.google.com/store/apps/details?id=com.jikoapps.charto&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img
              alt='Get it on Google Play'
              src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png'
            /></a>
            <h3>使用技術</h3>
            <div class="techs">
              <div>
                <img src="~/static/vue.png"/>
                <p>Vue.js</p>
              </div>
              <div>
                <img src="~/static/firebase_logo.png"/>
                <p>Firebase</p>
              </div>
            </div>
          </Card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>
<style lang="scss" scoped>
  img {
    height: 100px;
  }

  .techs {
    display: flex;
    justify-content: space-around;

    > img {
      height: 200px;
    }
  }

  .card-text {
    text-align: left;
  }
</style>

<script>
  import Card from '~/components/Card.vue'
  import CharToHeader from '~/static/charto_header.png'
  import CharToWebHeader from '~/static/charto_web_header.png'
  import MarkparkHeader from '~/static/markpark_header.png'

  export default {
    name: "Apps.vue",
    components: {
      Card,
    },
    data() {
      return {
        charto_header: CharToHeader,
        charto_web_header: CharToWebHeader,
        markpark_header: MarkparkHeader,
      }
    }
  }
</script>

<style scoped>

</style>