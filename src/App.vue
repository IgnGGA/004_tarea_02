<template>
  <div id="nav">
    <router-link to="/home">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/contact">Contact</router-link> |
    <router-link to="/info">Info</router-link> |
    <router-link to="/registration">Registration</router-link> |
    <router-link to="/rules">Rules</router-link> |
  </div>
  <router-view />
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
  display: flex;
  border:solid;
  justify-content: center;
  a {
    font-weight: bold;
    color: #033540;

    &.router-link-exact-active {
      color: #0df205;
    }
  }
}
#Rules,.about,#Info,#Contact,.home{
  display: flex;
  flex-direction: column;
  text-align:justify;
  h1,h2,h3,p{
    text-align:center;
  }
}
#infotable{
  display: flex;
  justify-content: center;
  text-align: center;
}
#Registration{
  display: flex;
  fieldset{
    margin-top:3%
  }
  input,label{
    margin-bottom:1%;
  }
}
</style>
