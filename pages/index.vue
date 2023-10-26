<template>
  <v-row justify='center' align='center'>
    <v-col cols='12' sm='8' md='6'>
      <Wellcome />
    </v-col>
  </v-row>
</template>

<script>
import Wellcome from '@/components/Wellcome'

export default {
  name: 'HomePage',
  components: { Wellcome }
}
</script>
