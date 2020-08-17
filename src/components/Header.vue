<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">About</a>
          </li>

          <li class="nav-item">
            <a class="nav-link" href="#">Contacts</a>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Lato&display=swap");

* {
  box-sizing: border-box;
}

img {
  width: auto;
  max-height: 80px;
}
.navbar {
  box-shadow: 0 0.1875rem 1.5rem rgba(0, 0, 0, 0.2);
  background-color: white !important;
}

.navbar-brand {
  margin: 0px 0px 0px 30px;
  padding: 0px 15px;
}

.nav-link {
  font-family: "Lato";
  font-size: 16px;
  font-weight: 500;
  text-transform: uppercase;
  padding: 15px !important;
  color: black !important;
}
</style>
