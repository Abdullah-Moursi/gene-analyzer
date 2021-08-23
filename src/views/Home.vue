<template>
  <div class="cont">
    <HomeNavigation />
    <div>
      <div class="home row col-12 justify-content-center px-0 m-0">
        <h1>GENE ANALYZER</h1>
      </div>
    </div>
    <div class="img">
      <img src=".././images/chromosome.jpg" />
    </div>
  </div>
</template>

<script>
import HomeNavigation from "@/components/HomeNavigationBar.vue";

export default {
  name: "Home",
  components: {
    HomeNavigation,
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
.img {
  margin-top: 80px;
}
img {
  max-width: 800px;
  max-height: 700px;
  border-radius: 5%;
}
</style>
