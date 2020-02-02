<template>
  <h2>Emitの実装</h2>
  <my-input @input="onInput"/>
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
    const msg = ref('こんにちは')

    const onInput = ($event) => {
      msg.value = $event
    }
    return {
      msg,
      onInput
    }
  }
}
</script>

<style scoped>
img {
  width: 200px;
}
h1 {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
