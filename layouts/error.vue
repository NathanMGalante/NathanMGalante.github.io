<template>
  <v-app>
    <v-container class='text-center'>
      <h1>
        {{ isNotFoundError ? pageNotFound : otherError }}
      </h1>
      <NuxtLink to='/'>Home page</NuxtLink>
    </v-container>
  </v-app>
</template>

<script>
export default {
  name: 'EmptyLayout',
  layout: 'empty',
  props: {
    error: {
      type: Object,
      default: null
    }
  },
  data: () => ({
    pageNotFound: '404 Not Found',
    otherError: 'An error occurred'
  }),
  computed: {
    isNotFoundError() {
      return this.error.statusCode === 404
    }
  },
  head: (vm) => ({
    title: vm.isNotFoundError ? vm.pageNotFound : vm.otherError
  })
}
</script>

<style scoped>
h1 {
  font-size: 20px;
}
</style>
