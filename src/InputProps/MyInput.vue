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
    return {
    }
  }
}
</script>
