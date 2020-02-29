<template>
  <v-layout column>
    (省略)
    <!-- HTML タグ の 形式 で 埋め込める！ -->
    <!-- v-for で この タグ を 繰り返し 出力 できる -->
    <form-card v-for="i in 11" :key="`${i}`"/>
    <v-btn @click="submit">診断結果を表示する</v-btn>
  </v-layout>
</template>

<script lang="ts">

import {Vue, Component} from 'nuxt-property-decorator'
// デコレータ内で、このコンポーネントを
// 使うことを宣言し、同時にimport

@Component({
  components: {
    FormCard: () => import('../components/FormCard.vue')
  }})
  export default class Index extends Vue { }
</script>
