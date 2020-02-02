<template>
  <input type="text" @input="onInput"/>
</template>

<script>
import { ref } from 'vue'

export default {
  props: {
    value: {
      type: String,
      default: ''
    }
  },
  setup(props, context) {
    const onInput = ($event) => {
      context.emit('input', $event.target.value)
    }
    return {
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
