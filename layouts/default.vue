<template>
  <v-app>
    <BackgroundImage />
    <v-app-bar fixed app>
      <v-toolbar-title>{{ title }}</v-toolbar-title>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer app>
      <span>&copy; {{ currentYear }}</span>
    </v-footer>
  </v-app>
</template>

<script>
import { getYear } from '@/utils/date-util'
import BackgroundImage from '@/components/BackgroundImage'

export default {
  name: 'DefaultLayout',
  components: { BackgroundImage },
  data: () => ({
    title: 'Nathan Moreno Galante',
    currentYear: getYear()
  })
}
</script>
