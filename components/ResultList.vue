
<template>
  <v-list two-line>
    <template v-for="w in wineAttr">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title>酒石酸 濃度</v-list-item-title>
          <v-list-item-subtitle>fixed acidity</v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action>
          <v-list-item-action-text>0.1</v-list-item-action-text>
        </v-list-item-action>
      </v-list-item>
      <v-divider></v-divider>
    </template>
  </v-list>
</template>

<script lang="ts">
import { Vue, Component } from 'nuxt-property-decorator'
@Component
export default class extends Vue {
  get wineAttr() {
    return [1,2,3,4,5,6,7,8,9,10];
  }
}
</script>
