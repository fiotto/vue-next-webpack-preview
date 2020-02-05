<template>
  <h2>v-modelの実装</h2>
  <my-input v-model="msg"/>
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
    const msg = ref('こんばんは')

    return {
      msg
    }
  }
}
</script>
