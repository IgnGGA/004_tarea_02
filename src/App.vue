<template>
  <div id="nav">
    <router-link to="/home">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #033540;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #033540;

    &.router-link-exact-active {
      color: #0DF205;
    }
  }
}
</style>
