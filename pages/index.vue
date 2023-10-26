<template>
  <v-row justify='center' align='center'>
    <v-col cols='12' sm='8' md='6'>
      <v-card class='text-center ma-4'>
        <h3>Em desenvolvimento...</h3>
      </v-card>
      <Wellcome />
      <BubbleImage />
    </v-col>
  </v-row>
</template>

<script>
import BubbleImage from '@/components/BubbleImage'
import Wellcome from '@/components/Wellcome'

export default {
  name: 'HomePage',
  components: { BubbleImage, Wellcome }
}
</script>
