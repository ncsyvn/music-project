<template>
  <div>
    <div class="flexbox">
      <!-- Sidebar area -->
      <side-bar></side-bar>
      <div class="full-width">
        <Header></Header>
        <div class="main-page">
          <!-- Search area -->
          <div class="search-div">
            <div class="search-area">
              <input
                type="text"
                class="txt-input-search"
                placeholder="Search for new music, news, artists..."
              />
              <img src="../src/assets/icons/search.png" class="icon-search" />
            </div>
          </div>
          <!-- Trending area -->
          <div></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./components/common/Header.vue";
import SideBar from "./components/common/SideBar.vue";

export default {
  name: "App",
  components: {
    SideBar,
    Header,
  },
};
</script>

<style scoped>
@import "../src/css/common.css";
@import "../src/css/home-page.css";
</style>
