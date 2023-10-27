<template>
  <v-app>
    <v-app-bar fixed app>
      <v-toolbar-title>{{ title }}</v-toolbar-title>
    </v-app-bar>
    <v-main>
      <v-container class='page' fluid>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer app>
      <span>&copy; {{ currentYear }}</span>
      <v-row no-gutters justify='center'>&nbsp;Em Desenvolvimento...</v-row>
    </v-footer>
  </v-app>
</template>

<script>
import { getYear } from '@/utils/date-util'

export default {
  name: 'DefaultLayout',
  data: () => ({
    title: 'Nathan Moreno Galante',
    currentYear: getYear()
  })
}
</script>
