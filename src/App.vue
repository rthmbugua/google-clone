<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view />-->
    <NavBar></NavBar>

    <img style="max-width:20em;height:auto" src="./assets/gogglelogo.png" alt />
    <searchBar style="margin-top:6em;" />
    <Favourite style="margin-top:2em;" />
  </div>
</template>
<script>
import NavBar from "./components/NavBar";
import SearchBar from "./components/SearchBar";
import Favourite from "./components/Favourites";
export default {
  name: "app",
  components: {
    NavBar,
    SearchBar,
    Favourite
  }
};
</script>
<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
  display: flex;
  align-items: center;
  flex-direction: column;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
.nav-bar {
  line-height: 6em;
  width: 100%;
  display: flex;
  justify-content: flex-end;
}
.words {
  margin: 1em 0.5em 1em 0.5em;
  font-size: 15px;
}
.favourite {
  display: flex;
  flex-flow: row wrap;
  align-content: center;
  width: 36%;
}
.fav {
  margin: 1em;
  text-align: center;
}
</style>
