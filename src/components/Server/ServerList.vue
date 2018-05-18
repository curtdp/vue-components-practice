<template>
  <div class="col-xs-12 col-sm-6">
    <ul class="list-group">
      <ServerListItem v-for="server in servers" :id="server.id" :key="server.id"></ServerListItem>
    </ul>
  </div>
</template>

<script>
  import ServerListItem from './ServerListItem.vue'
  export default {
    data() {
      return {
        servers: [
          { id: 1, status: 'Normal'},
          { id: 2, status: 'Critical'},
          { id: 3, status: 'Unknown'},
          { id: 4, status: 'Normal'},
        ]
      }
    },
    components: {
      ServerListItem
    }
  }
</script>

<style scoped>
  div {
    border: 1px solid blue;
  }
</style>
