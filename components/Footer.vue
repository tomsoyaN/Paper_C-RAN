<script>
export default {
  props: {
    author: {
      
    },
    title: {
      type: String,
    }
  }
}
</script>

<template>
  <div  class="bg-barBottom flex absolute w-full bottom-0 left-0 py-0.5 px-4 text-sm ">
    <div class="w-1/3 text-left">
      {{ author }}
    </div>
    <div class="w-1/3 text-left">
      {{ title }}
    </div>
    <div class="w-1/3 flex justify-end">
      {{ $slidev.nav.currentPage }} / {{ $slidev.nav.total }}
    </div>
  </div>
</template>