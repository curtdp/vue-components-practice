<template>
  <div class="col-xs-12 col-sm-6">
    <p>Server Details Currently not updated</p>
  </div>
</template>

<script>
  import { serverBus } from '../../main.js';
  export default {
    data() {
      return {
        server: null
      }
    },
    created() {
      serverBus.$on('serverSelected', (server) => {
        this.server = server;
      });
    }
  }
</script>

<style scoped>
  div {
    border: 1px solid red;
  }
</style>