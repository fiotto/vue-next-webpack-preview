<template>
  <input-props></input-props>
  <input-emit></input-emit>
  <input-sync></input-sync>
</template>

<script>
import InputProps from './InputProps/Index.vue'
import InputEmit from './InputEmit/Index.vue'
import InputSync from './InputSync/Index.vue'

export default {
  components: {
    InputProps,
    InputEmit,
    InputSync
  }
}
</script>

