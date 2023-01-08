<template>
  <header>
    <h1>{{propsdata}}</h1>
    <button v-on:click="sendEvnet">Send</button>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  props: ['propsdata'],
  methods: {
    sendEvnet: function () {
      this.$emit('renew')
    }
  }
}
</script>

<style scoped>

</style>