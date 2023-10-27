<template>
  <v-row>
    <v-col class='white black--text'>
      <h1>{{ title }}</h1>
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
