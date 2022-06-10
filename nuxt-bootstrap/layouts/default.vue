<template>
  <div id="app">
 <header-part/>
    <nuxt/>
  </div>
</template>

<script>
import HeaderPart from "~/components/HeaderPart.vue"
export default {
  components: {
    HeaderPart
  }
}
</script>
