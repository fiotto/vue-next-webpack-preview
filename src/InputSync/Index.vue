<template>
  <h2>Syncの実装</h2>
  <my-input v-model:value="msg"/>
  <p>{{ msg }}</p>
</template>

<script>
import { ref } from 'vue'

import MyInput from './MyInput.vue'

export default {
  components: {
    MyInput
  },
  setup() {
    const msg = ref('おやすみ')

    return {
      msg
    }
  }
}
</script>
