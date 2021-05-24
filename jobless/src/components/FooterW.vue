<template>
  <div id="footerW">
    <div class="container">
      <div class="row">
        <div class="col-sm">
          <router-link to="/about" class="about">About</router-link>
        </div>
        <div class="col-sm">
          <img src="../assets/Jobless logo mali.png" id="home-logo" alt="" />
        </div>
        <div class="col-sm">
          <span v-bind:title="year">Jobless &copy; {{ year }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterW",
  data() {
    return {
      year: new Date().getFullYear(),
    };
  },
};
</script>

<style lang="scss" scoped>
#footerW {
  background-color: #d9d9d9;
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
#home-logo {
  height: 28px;
}
.about {
  color: black;
  text-decoration: none;
}
</style>
