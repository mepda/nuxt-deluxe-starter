<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <nuxt-link to="/">
        <img
          src="/mini_logo.png"
          id="Logo__image"
          width="75"
          height="25"
          alt="Uninja Logo"
        />
      </nuxt-link>
      <nuxt-link to="/" id="logo_name">Zelas</nuxt-link>
      <a
        role="button"
        class="navbar-burger burger"
        @click="isActive = !isActive"
        :class="{ 'is-active': isActive }"
        aria-label="menu"
        aria-expanded="false"
        data-target="navbarBasicExample"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div
      id="navbarBasicExample"
      class="navbar-menu"
      :class="{ 'is-active': isActive }"
    >
      <div class="navbar-start"></div>
      <div class="navbar-end">
        <div class="navbar-item">
          <label class="switch">
            <input type="checkbox" />
            <span class="slider round languages">En Es</span>
          </label>
          <nuxt-link to="/" class="navbar-item">Home</nuxt-link>
          <nuxt-link to="/about" class="navbar-item">About</nuxt-link>
          <hr class="navbar-divider" />
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isActive: false
    };
  },
  methods: {
    toggleHamburgerMenu() {
      isActive ? false : true;
    }
  }
};
</script>

<style scoped>
.navbar {
  background: #2196f3;
}
#logo_name {
  font-size: 22px;
}

#Logo__image {
  height: 45px;
  width: auto;
}

#logo_name:hover,
.navbar-item:hover,
.nuxt-link-active {
  background: initial !important;
  color: white !important;
}

.navbar-brand {
  display: flex;
  justify-content: center;
  align-items: center;
}
.navbar-brand img {
  margin: 5px 5px 0 0;
  padding: 0 5px;
}
.navbar-end {
  display: flex;
  align-items: center;
}
.switch {
  position: relative;
  display: inline-block;
  width: 60px;
  height: 34px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}
.slider:hover {
  color: white !important;
}
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 26px;
  width: 26px;
  left: 4px;
  bottom: 4px;
  background-color: whitesmoke;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

input:checked + .slider {
  background-color: #2196f3;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2196f3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
  color: black;
  font-size: 17px;
}

.slider.round:before {
  border-radius: 50%;
}

.languages {
  display: flex;
  justify-content: center;
  align-items: center;
}
@media screen and (max-width: 1023px) {
  .navbar-menu {
    background-color: darkgray;
  }
}
@media (max-width: 800px) {
  .navbar-item {
    font-size: 16px !important;
  }
}
.navbar-brand span,
.navbar-item {
  font-size: 22px;
}
.navbar-item,
.navbar-link {
  color: whitesmoke !important;
}
</style>
