<template>
  <div class="boja">
    <div class="container">
      <div class="row">
        <div
          class="col-md-12 col-12"
          style="margin-top: 50px; margin-bottom: 15px"
        >
          <h1
            style="
              font-size: 75px;
              text-align: center;
              text-shadow: 6px 6px 8px #a0a0a0;
              font-family: Papyrus Copperplate Fantasy;
            "
          >
            Sign up
          </h1>
        </div>
        <div class="col-md-12">
          <form style="margin-top: 15px">
            <div class="form-group">
              <label for="name_signup" class="center">Name:</label>
              <input
                type="text"
                class="form-control center"
                id="name_signup"
                placeholder="Enter name..."
                style="height: 48px"
              />
            </div>
            <div class="form-group">
              <label for="surname_signup" class="center">Surname:</label>
              <input
                type="text"
                class="form-control center"
                id="surname_signup"
                placeholder="Enter surname..."
                style="height: 48px"
              />
            </div>

            <label for="type_user" class="center">Type of User:</label>
            <select
              class="form-select center"
              aria-label="Default select example"
              style="height: 48px; margin-bottom: 25px"
              id="type_user"
            >
              <option value="buyer">Buyer</option>
              <option value="seller">Seller</option>
            </select>
            <div class="form-group">
              <label for="username_signup" class="center">Username:</label>
              <input
                type="text"
                class="form-control center"
                id="username_signup"
                placeholder="Enter username..."
                style="height: 48px"
              />
            </div>
            <div class="form-group">
              <label for="email_signup" class="center">Email:</label>
              <input
                type="email"
                class="form-control center"
                id="email_signup"
                placeholder="Enter email..."
                style="height: 48px"
              />
            </div>
            <div class="form-group">
              <label for="pass_signup" class="center">Password:</label>
              <input
                type="password"
                class="form-control center"
                id="pass_signup"
                placeholder="Enter password..."
                style="height: 48px"
              />
            </div>
            <div class="form-group">
              <label for="confirmpass_signup" class="center"
                >Confirm password:</label
              >
              <input
                type="password"
                class="form-control center"
                id="confirmpass_signup"
                placeholder="Confirm password..."
                style="height: 48px"
              />
            </div>
            <button
              class="btn btn-outline-dark center"
              type="submit"
              style="height: 40px; margin-top: 5px; width: 80px"
            >
              Signup
            </button>
          </form>
        </div>
      </div>
    </div>
    <div class="slika_centrirano"><img src="@/assets/logo.jpg" /></div>
  </div>
</template>

<script>
export default {
  name: "Signup",
};
</script>
<style scoped>
.slika_centrirano {
  display: flex;
  justify-content: center;
}
.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 40%;
}
.boja {
  background-color: #ebebeb;
}

label {
  font-size: 20px;
}
</style>
