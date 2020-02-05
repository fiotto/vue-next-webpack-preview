<template>
  <input type="text" :value="value" @input="onInput"/>
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
      context.emit('update:value', $event.target.value)
    }
    return {
      onInput
    }
  }
}
</script>
