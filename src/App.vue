<template>
    <div class="container">
        <Header></Header>
        <hr>
        <div class="row">
          <ServerList></ServerList>
          <ServerStatus></ServerStatus>
        </div>
        <Footer></Footer>
    </div>
</template>

<script>
  import Header from './components/Shared/Header.vue'
  import Footer from './components/Shared/Footer.vue'
  import ServerStatus from './components/Server/ServerStatus.vue'
  import ServerList from './components/Server/ServerList.vue'
    export default {
      components: {
        Header,
        Footer,
        ServerStatus,
        ServerList
      }
    }
</script>

<style>

</style>
