<!-- <template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style> -->

<template>
  <div id="app">
    <div>
      <b-navbar class="navbar-green">
        <b-navbar variant="faded" type="light">
          <b-navbar-brand class="navbar_logo" href="#">
            <img
              src="2id logo.png"
              class="d-inline-block align-top brand-image"
              alt="2id-logo"
            />
            <div class="brand-div">
              <h2 class="brand-title">2nd Infantry Division</h2>
              <span class="brand-subtitle">Home of the Jungle Fighter</span>
            </div>
          </b-navbar-brand>
        </b-navbar>
        <b-navbar-nav class="ms-auto">
          <router-link class="nav-item" to="/">Home</router-link>
          <router-link class="nav-item" to="/about">About</router-link>
          <router-link class="nav-item" to="/">Join the Army</router-link>
          <router-link class="nav-item" to="/">Contact</router-link>
          <!-- Navbar dropdowns -->
          <!-- <b-nav-item-dropdown text="About" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown text="User" right>
            <b-dropdown-item href="#">Account</b-dropdown-item>
            <b-dropdown-item href="#">Settings</b-dropdown-item>
          </b-nav-item-dropdown> -->
        </b-navbar-nav>
      </b-navbar>
    </div>

    <router-view />
  </div>
</template>
<style lang="css">
#app {
  background-color: #d8e9a8;
}

.navbar-green {
  background-color: #1e5128;
  padding: 0.5rem 2rem;
}

.navbar_logo {
  display: flex;
  align-items: center;
}

.brand-image {
  width: 60px;
}

.brand-div {
  color: white;
  margin-left: 8px;
}

.brand-title {
  font-size: 32px;
  margin-bottom: -8px;
  font-family: "Black Ops One";
}

.brand-subtitle {
  font-size: 16px;
  text-transform: uppercase;
  font-weight: bold;
  letter-spacing: 2px;
}

.nav-item {
  color: white;
  font-weight: bold;
  letter-spacing: 1px;
  text-decoration: none;
  padding-bottom: 5px;
  margin-right: 18px;
  border-bottom: 1px solid #1e5128;
  text-transform: uppercase;
}

.nav-item:hover {
  border-bottom: 1px solid white;
  text-decoration: none;
  color: white;
}

.nav-item:last-child {
  margin-right: 0;
}
</style>
