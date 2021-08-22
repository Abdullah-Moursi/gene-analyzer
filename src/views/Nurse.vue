<template>
  <div>
    <div class="cont">
      <HomeNavigation />
      <div>
        <h1>Add a Patient</h1>
        <div class="home row col-12 justify-content-center px-0 m-0">
          <form class="row gy-2 gx-3 align-items-center">
            <div class="col-auto">
              <label class="visually-hidden" for="autoSizingInput">Name</label>
              <input
                type="text"
                v-model="name"
                class="form-control"
                id="autoSizingInput"
                placeholder="Patient Name"
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
              <label class="visually-hidden" for="autoSizingInput">DNA</label>
              <input
                type="text"
                v-model="DNA"
                class="form-control"
                id="autoSizingInput"
                placeholder="DNA"
              />
            </div>

            <div class="col-auto">
              <button @click="AddPatient" type="submit" class="btn btn-primary">
                Submit
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HomeNavigation from "@/components/HomeNavigationBar.vue";

export default {
  name: "Nurse",
  components: {
    HomeNavigation,
  },
  data() {
    return {
      name: "",
      ID: "",
      DNA: "",
    };
  },
  methods: {
    AddPatient(e) {
      const newPatient = {
        name: this.name,
        ID: this.ID,
        DNA: this.DNA,
      };
      e.preventDefault()
      console.log(newPatient);
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
.BROWS {
  background-color: rgb(16, 17, 17);
  width: 100px;
  height: 100px;
  margin-top: 400px;
}
</style>
