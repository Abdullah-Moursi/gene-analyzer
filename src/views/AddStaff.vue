<template>
  <div>
    <div class="cont">
      <HomeNavigation />
      <div>
        <h1>Add Staff</h1>
          <form class="row gy-2 gx-3 align-items-center">
            <div class="col-auto">
              <label class="visually-hidden" for="autoSizingInput">Name</label>
              <input
                type="text"
                v-model="name"
                class="form-control"
                id="autoSizingInput"
                placeholder="Name"
              />
            </div>
            <div class="col-auto">
              <label class="visually-hidden" for="autoSizingInput">ID</label>
              <input
                type="number"
                v-model="ID"
                class="form-control"
                id="autoSizingInput"
                placeholder="ID"
              />
            </div>
            <div class="col-auto">
              <label class="visually-hidden" for="autoSizingInput">Password</label>
              <input
                type="text"
                v-model="Password"
                class="form-control"
                id="autoSizingInput"
                placeholder="Password"
              />
            </div>

            <div class="col-auto">
              <button @click="AddMember" type="submit" class="btn btn-primary">
                Add
              </button>
            </div>
          </form>
      </div>
    </div>
  </div>
</template>

<script>
import HomeNavigation from "@/components/HomeNavigationBar.vue";

export default {
  name: "AddStaff",
  components: {
    HomeNavigation,
  },
  data() {
    return {
      name: "",
      ID: "",
      Password: "",
    };
  },
  methods: {
    AddMember(e) {
      const newMember = {
        name: this.name,
        ID: this.ID,
        Password: this.Password,
      };
      e.preventDefault()
      console.log(newMember);
      this.name = '';
      this.ID = '';
      this.Password = '';
    },
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

.col-auto {
  margin: 20px auto;
}
</style>
