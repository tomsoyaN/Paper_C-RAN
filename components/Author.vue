<template>
    
</template>
<script lang="ts">
import { provide,inject,defineComponent } from 'vue'
import {SlideInfo,KeySlideInfo} from './Initialize.vue'
export default defineComponent({
    setup(){
      const info = inject(KeySlideInfo)
      console.log(info)
    }
})
</script>