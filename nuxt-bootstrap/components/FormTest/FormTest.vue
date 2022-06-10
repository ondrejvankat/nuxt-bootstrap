<template>
  <div>

    <p>Message is: {{ message }}</p>
    <input v-model="message" placeholder="edit me" />


  </div>
</template>

<script>
export default {
  data () {
    return {
      message: ''
    }
  }
}
</script>
