<template>
  <div @click="handleImport">{{msg}}</div>
</template>

<script>
export default {
  data() {
    return {
      msg: 'this is vue2qqqxxxx'
    }
  },
  methods: {
    async handleImport() {
      await import(/* webpackChunkName: "lodash" */ /* webpackPrefetch: true */ 'lodash');
    }
  }
}
</script>

<style lang="scss" scoped>
div{
  color: red;
}
</style>