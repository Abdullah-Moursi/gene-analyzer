<template>
  <div class="cont">
    <HomeNavigation />
    <div>
      <div class="home row col-12 justify-content-center px-0 m-0">
        <h3>Login</h3>
      </div>
    </div>
  </div>
</template>

<script>
import HomeNavigation from "@/components/HomeNavigationBar.vue";

export default {
  name: "Login",
  components: {
    HomeNavigation
  },
};
</script>

<style scoped>
.cont {
  height: calc(200vh);
  background-color: rgb(133, 167, 187);
}
.home {
  background-repeat: no-repeat;
  height: calc(70vh);
  width: 100%;
  background-position: center;
  background-size: 100% 100%;
  position: absolute;
}
.BROWS {
  background-color: rgb(16, 17, 17);
  width: 100px;
  height: 100px;
  margin-top: 400px;
}
</style>
