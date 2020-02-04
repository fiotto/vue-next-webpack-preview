<template>
  <input type="text" :value="value"/>
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
  setup(props) {
    const onInput = ($event) => {
      context.emit('update:value', $event.target.value)
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
