<template>
  <div>
    <div class="flexbox">
      <!-- Sidebar area -->
        <side-bar></side-bar>
        <div class="full-width">
          <Header></Header>
          <div class="main-page">
          </div>
        </div>
    </div>
  </div>
</template>

<script>
import Header from './components/common/Header.vue'
import SideBar from './components/common/SideBar.vue'

export default {
  name: 'App',
  components: {
    SideBar,
    Header
  }
}
</script>

<style scoped>
  @import "../src/css/common.css"
</style>
