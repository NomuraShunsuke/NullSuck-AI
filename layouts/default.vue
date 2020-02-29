<template>
  <v-app>
    <v-app-bar
      fixed
      app
      color="primary"
      class="white--text"
    >
      <v-app-bar-nav-icon class="white--text"/>
      <v-toolbar-title text="入力"/>
    </v-app-bar>
    <v-content>
      <v-container>
        <nuxt/>
      </v-container>
    </v-content>
    <v-footer app>
      <span>&copy; 2019 Norwegian Geek </span>
    </v-footer>
  </v-app>
</template>

< script lang ="ts">
  //この中にTypeScriptを記載する
  import {Vue, Component} from 'nuxt-property-decorator'

  @Component
  export default class Layout extends Vue {}
</script>

<style scoped>
  /* この中にCSSを記載してstyleを定義 */
</style>
