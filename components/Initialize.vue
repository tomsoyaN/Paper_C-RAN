<template>
    
</template>
<script lang="ts">
import { provide,InjectionKey,reactive,defineComponent } from 'vue'

export interface SlideInfo{
    author:string,
    section:string,
}

export const KeySlideInfo:InjectionKey<SlideInfo> =   Symbol('SlideInfo')

export default defineComponent({
    setup(){
        const info:SlideInfo = reactive<SlideInfo>({author:'',section:''})
    provide(KeySlideInfo,info)
    console.log("Init Slide")
    }
})
</script>