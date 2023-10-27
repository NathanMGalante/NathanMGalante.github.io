<template>
  <v-row class='white black--text' justify='center'>
    <v-col cols='8' class='py-6'>
      <h1 class='dark-blue--text'>{{ title }}</h1>
      <slot />
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'Info',
  props: {
    title: {
      type: String,
      required: true
    }
  }
}
</script>
