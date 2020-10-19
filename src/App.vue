<template>
  <div id="app">
    <div id="nav">
      <top-header />
    </div>
    <router-view />
  </div>
</template>


<script>
import TopHeader from "./components/TopHeader.vue";
export default {
  components: {
    "top-header": TopHeader
  }
};
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  font-size: 1.2rem;
  color: #000000;
}

#nav {
  padding: 10px;
  font-size: 1.3rem;
  a {
    font-weight: bold;
    color: #000000;

    &.router-link-exact-active {
      color: #f31717;
    }
  }
}
</style>
