<template>
  <nav
    class="navbar navbar-expand-lg navbar-light"
    style="background-color: #d2c1a7"
  >
    <div class="container-fluid">
      <div>
        <img src="@/assets/pozadina.jpg" style="width: 50px; height: 50px" />
      </div>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link to="/" class="nav-link active">Home</router-link>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link active dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              Products
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <a class="dropdown-item" href="/paintings">Paintings</a>
              <a class="dropdown-item" href="/sculptures">Sculptures</a>
              <a class="dropdown-item" href="/comics">Comics</a>
              <a class="dropdown-item" href="/books">Books</a>
              <a class="dropdown-item" href="/coins">Coins</a>
              <a class="dropdown-item" href="/maps">Maps</a>
              <a class="dropdown-item" href="/raresignatures">Rare signature</a>
              <a class="dropdown-item" href="/productssignedbycelebrities"
                >Products signed by celebrities</a
              >
              <a class="dropdown-item" href="/cards">Cards</a>
            </div>
          </li>
          <li class="nav-item">
            <router-link to="/" class="nav-link active">Logout</router-link>
          </li>
        </ul>
        <form class="d-flex">
          <input
            v-model="store.searchTerm"
            class="form-control me-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
            style="margin-top: 5px"
          />

          &nbsp;
          <a href="/cart"
            ><i
              class="fas fa-shopping-cart fa-2x nav-link active"
              style="color: black"
            >
            </i
          ></a>
          <a href="/myprofile"
            ><i
              class="fas fa-user-circle fa-2x nav-link active"
              style="color: black"
            ></i
          ></a>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
import store from "@/store.js";
export default {
  name: "navbar_buyer",
  data() {
    return {
      store: store,
    };
  },
};
</script>
