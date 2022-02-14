<template>
  <div class="sidebar">
    <button class="btn_logo">
      <img
        src="../../assets/images/logo.png"
        width="72"
        height="54"
        @click="logoutClick"
      />
    </button>

    <div class="menu">
      <button class="btn_sidebar_option">
        <img
          src="../../assets/icons/home.png"
          width="22"
          height="22"
          @click="logoutClick"
        />
      </button>
      <button class="btn_sidebar_option">
        <img
          src="../../assets/icons/chart.png"
          width="22"
          height="22"
          @click="logoutClick"
        />
      </button>
      <button class="btn_sidebar_option">
        <img
          src="../../assets/icons/files.png"
          width="22"
          height="22"
          @click="logoutClick"
        />
      </button>
      <button class="btn_sidebar_option">
        <img
          src="../../assets/icons/chat.png"
          width="22"
          height="22"
          @click="logoutClick"
        />
      </button>
    </div>
    <hr />
    <div class="footer-sidebar">
      <button class="btn-help txt-language">Help</button>
      <select class="select-language txt-language">
        <option class="txt-language">EN</option>
        <option class="txt-language">VI</option>
      </select>
    </div>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  data: function () {
    return {
      amount_people_listening: 8,
      username: "Carlos López",
      job: "Artist",
    };
  },
};
</script>

<style scoped>
@import "../../css/common.css";
@import "../../css/sidebar.css";
</style>
