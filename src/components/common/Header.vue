<template>
  <div class="header">
    <div class="flexbox">
      <img
        src="../../assets/icons/icon_listen_music.png"
        width="20"
        height="20"
        class="icon-listen-music"
      />
        <p class="amount-people-listen">{{amount_people_listening}} people listen to you</p>
    </div>
    <div class="right-component">
        <div class="flexbox align-center-vertical">
          <div>
            <p class="txt-username">{{username}}</p>
            <p class="txt-job">{{job}}</p>
          </div>
          <button class="btn-avatar">
            <img src="../../assets/images/default_avatar.png" alt="Avatar" width=55 height=55 @click="avatarClick">
          </button>          
          <button class="btn-dropdown">
            <img src="../../assets/icons/drop_down.png" width=24 height=24 @click="dropdownClick">
          </button>
          <div class="border-left"></div>
          <button class="btn-notification">
            <img src="../../assets/icons/notification.png" width=24 height=24 @click="notificationClick">
          </button>
          <button class="btn-notification">
            <img src="../../assets/icons/logout.png" width=24 height=24 @click="logoutClick">
          </button>

        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data: function () {
    return {
      amount_people_listening: 8,
      username: "Carlos López",
      job: "Artist"
    };
  },
  methods: {
    avatarClick(){
      alert("Clicked avatar");
    },
    dropdownClick(){
      alert("Clicked dropdown");
    },
    notificationClick(){
      alert("Clicked notification");
    },
    logoutClick(){
      alert("Clicked logout");
    }
  }
};
</script>

<style scoped>
@import "../../css/common.css";
@import "../../css/header.css";
</style>
