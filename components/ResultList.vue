<template>
  <v-list two-line>
    <template v-for="i in 11" :key="`${i}`">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title>酒石酸 濃度</v-list-item-title>
          <v-list-item-subtitle>fixed acidity</v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action>
          <v-list-item-action-text>0. 1</v-list-item-action-text>
        </v-list-item-action>
      </v-list-item>
      <v-divider></v-divider>
    </template>
  </v-list>
</template>
