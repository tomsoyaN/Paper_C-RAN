<template>
  <div class="slidev-layout default">
    <slot />
    <Footer :title=section :author=author />
  </div>
</template>

<script>
import { defineComponent,getCurrentInstance } from 'vue'
export default defineComponent({
  props: {
    section: {
      type: String,
      default:'section'
    },
    author: {
      type: String,
      default:'author'
    },
  },
  setup(props,context) {
    return {
    }
  },
})
</script>

