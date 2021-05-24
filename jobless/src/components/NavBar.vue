<template>
  <div id="nav">
    <router-link to="/"
      ><img src="../assets/Jobless logo.png" id="home-logo" alt=""
    /></router-link>
    <span id="kIme">Korisničko ime</span>
    <span id="userIcon" class="material-icons">account_circle</span>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  props: {
    user_status: Boolean,
  },
};
</script>

<style lang="scss" scoped>
#nav {
  display: flex;
  align-items: center;
  //padding: 30px;
  max-height: 60px;
  justify-content: space-between;
  background-color: #d9d9d9;
  /* box-shadow: 0em 2px .75em #111; */
}
.material-icons {
  font-family: "Material Icons";
  font-weight: normal;
  font-style: normal;
  font-size: 30px; /* Preferred icon size */
  display: inline-block;
  line-height: 1;
  text-transform: none;
  letter-spacing: normal;
  word-wrap: normal;
  white-space: nowrap;
  /* Support for all WebKit browsers. */
  -webkit-font-smoothing: antialiased;
  /* Support for Safari and Chrome. */
  text-rendering: optimizeLegibility;
  /* Support for Firefox. */
  -moz-osx-font-smoothing: grayscale;
  /* Support for IE. */
  font-feature-settings: "liga";
}
#home-logo {
  height: 60px;
  
}

#kIme {
  padding-left: 1150px;
}

#login,
#userIcon {
  color: #3DBC91;
  padding-right: 40px;
}
</style>

<style scoped>
#navBar {
  background-color: #d9d9d9;
}
</style>
