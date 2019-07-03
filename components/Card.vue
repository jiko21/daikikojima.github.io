<template>
  <v-card>
    <v-img
      :src="image"
    ></v-img>

    <v-card-title primary-title>
      <div>
        <div class="headline">{{title}}</div>
      </div>
    </v-card-title>

    <v-card-actions>
      <v-spacer/>
      <v-btn icon @click="show = !show">
        <v-icon>{{ show ? 'keyboard_arrow_up' :  'keyboard_arrow_down' }}</v-icon>
      </v-btn>
    </v-card-actions>
    <v-slide-y-transition>
      <v-card-text v-show="show">
        <slot/>
      </v-card-text>
    </v-slide-y-transition>
  </v-card>
</template>

<script>
  export default {
    name: "Card",
    props: [
      'title',
      'image'
    ],
    data: () => ({
      show: false,
    }),
  }
</script>

<style lang="scss" scoped>
</style>