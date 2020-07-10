<template>
  <header>
    <h1>{{ propsdata }}</h1>
    <button @click="sendEvent">send</button>
  </header>
</template>

<script>
export default {
  // props: ['propsdata']
  props: {
    propsdata: String,
  },
  methods: {
    sendEvent: function() {
      this.$emit('renew');
    }
  }
}
</script>

<style>

</style>