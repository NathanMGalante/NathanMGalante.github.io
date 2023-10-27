<template>
  <v-row>
    <v-col class='wellcome text-center'>
      <h1>Nathan Moreno Galante</h1>
      <v-row no-gutters justify='center' style='height: 26px'>
        <vue-typed-js
          :backDelay='backDelay'
          :backSpeed='speed'
          :strings='text'
          :typeSpeed:='speed'
          class='position-absolute'
          loop
        >
          <span class='typing' style='font-size: 26px' />
        </vue-typed-js>
      </v-row>
      <BubbleImage class='mt-12 pt-12' />
    </v-col>
  </v-row>
</template>

<script>
import Vue from 'vue'
import VueTypedJs from 'vue-typed-js'

import { DURATION_3_SECONDS, DURATION_50_MILLIS } from '@/utils/time-util'

Vue.use(VueTypedJs)
export default {
  name: 'Wellcome',
  data: () => ({
    text: [
      'Sou um desenvolvedor <b>Front-end<b/>',
      'Tenho experiência com <b>Vue.js<b/>',
      'Sou um desenvolvedor <b>Mobile</b>',
      'Tenho experiência com <b>Flutter</b>'
    ],
    speed: DURATION_50_MILLIS,
    backDelay: DURATION_3_SECONDS
  })
}
</script>
