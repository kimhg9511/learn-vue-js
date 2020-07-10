<template>
  <div id="app">
    <app-header :propsdata="str" v-on:renew="renewStr"/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
export default {
  data: function() {
    return {
      str: 'hi',
    }
  },
  components: {
    AppHeader,
  },
  methods: {
    renewStr: function() {
      this.str = 'Header'
    }
  }
}
</script>

<style>

</style>