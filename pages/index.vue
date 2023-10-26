<template>
  <v-row justify='center' align='center'>
    <v-col cols='12' sm='8' md='6'>
      <v-card class='text-center'>
        <h3>Em desenvolvimento...</h3>
      </v-card>
      <BubbleImage/>
    </v-col>
  </v-row>
</template>

<script>
import BubbleImage from '@/components/BubbleImage'

export default {
  name: 'HomePage',
  components: { BubbleImage }
}
</script>
