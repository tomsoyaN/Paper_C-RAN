<script>
export default {
  props: {
    author: {
      type:String
    },
    title: {
      type: String,
    },
    url:{
      type:String
    },
    access:{
      type:String
    }
  }
}
</script>

<template>
  <div>
    <p>{{ author }} 「{{ title }}」,</p>
    <p style="position:relative;bottom:15px;left:10%;line-height:100%;">[{{ url }}] {{ access }}アクセス.</p>
 </div>
</template>