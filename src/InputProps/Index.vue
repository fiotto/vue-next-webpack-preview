<template>
  <h2>Propsの実装</h2>
  <my-input :value="msg"/>
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
    const msg = ref('おはよう')

    return {
      msg
    }
  }
}
</script>
