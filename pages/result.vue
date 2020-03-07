<template>
  <v-layout column>
    <result-chart/>
    <result-list/>
    <v-btn @click="back">もう一度診断する</v-btn>
  </v-layout>
</template>

<script lang="ts">

import {Vue, Component} from 'nuxt-property-decorator'
// デコレータ内で、このコンポーネントを
// 使うことを宣言し、同時にimport

@Component({
  components: {
    ResultChart: () =>import('~/components/ResultChart.vue'),
    ResultList: () => import('~/components/ResultList.vue')
  }})
  export default class Result extends Vue { }
</script>
