<template>
  <div class="navbar-container justify-content-center">
    <div class="navbar-list">
      <ul>

        <router-link to="/" tag="li">
          <a>Home_page</a>
        </router-link>

        <router-link to="/Nurse" tag="li">
          <a>Nurse_page</a>
        </router-link>

        <router-link to="/Login" tag="li">
          <a>Login_page</a>
        </router-link>

              <router-link to="/DataManager" tag="li">
          <a>Data_manager</a>
        </router-link>

      </ul>
    </div>
  </div>
</template>

<script>

export default {
  name: "HomeNavigation"
};
</script>


<style scoped>
.navbar-container {
  width: 100%;
  margin: 0%;
  height: 80px;
  z-index: 2000;
}
ul {
  margin: 0%;
  list-style-type: none;
  display: inline-flex;
}
li {
  padding: 28px 17px;
  text-align: center;
  float: right;
  color: #ffffff;
}
a {
  color: #ffffff;
  font-size: 15px;
  text-decoration: none;
  padding: 0%;
  display: block;
}
a:hover {
  color: #0f0f0f;
}
#separator {
  color: #ffffff;
}
.navbar-list {
  background-color: rgb(37, 91, 122);
  width: 100%;
  font-family: Helvetica, Arial, sans-serif;
  font-size: 16px;
  font-weight: 700;
  line-height: 1.5;
  position: fixed;
  margin: 0;
}
#logout
{
  background-color:rgb(96, 155, 189);
  border-radius: 10px;
  height: 50px;
  margin-top: 20px;
}
</style>