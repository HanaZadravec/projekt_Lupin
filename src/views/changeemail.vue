<template>
  <navbar_buyer />
  <div class="container">
    <div class="row">
      <div class="col-md-12" style="margin-top: 50px; margin-bottom: 30px">
        <h1 style="font-family: Arial, Helvetica, sans-serif">
          <b
            >My profile<i
              class="fas fa-user-circle fa-sm nav-link active"
              style="color: black"
            ></i
          ></b>
        </h1>
      </div>
    </div>
  </div>
  <div class="container">
    <div class="row">
      <div class="col-md-4">
        <menu_myprofile />
      </div>
      <div class="col-md-1 vl"></div>
      <div class="col-md-7">
        <h2 style="font-family: Arial, Helvetica, sans-serif">
          <b>Change email address</b>
        </h2>

        <form style="margin-top: 15px">
          <div class="form-group">
            <label for="new_email">New email address:</label>
            <input
              type="email"
              class="form-control"
              id="new_email"
              placeholder="Enter new email..."
            />
          </div>
          <div class="form-group">
            <label for="confirm_newemail">Confirm new email address:</label>
            <input
              type="password"
              class="form-control"
              id="confirm_newemail"
              placeholder="Confirm new email address..."
            />
          </div>
          <div class="form-group">
            <label for="pass">Password:</label>
            <input
              type="password"
              class="form-control"
              id="pass"
              placeholder="Enter your current password..."
            />
          </div>

          <button type="button" class="btn btn-dark center" style="width: 80px">
            Update
          </button>
        </form>
      </div>
    </div>
  </div>
  <footer_app />
</template>

<script>
// @ is an alias to /src
import navbar_buyer from "@/components/navbar_buyer.vue";
import footer_app from "@/components/footer_app.vue";
import menu_myprofile from "@/components/menu_myprofile.vue";

export default {
  name: "Change email address",
  components: {
    navbar_buyer,
    footer_app,
    menu_myprofile,
  },
};
</script>
<style scoped>
.vl {
  border-left: 2px solid black;
  height: 500px;
}
.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}
@media screen and (max-width: 767.5px) {
  .col-md-1 {
    display: none;
  }
  .col-md-7 {
    margin-top: 30px;
  }
}
</style>
