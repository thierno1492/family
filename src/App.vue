<template>
  <div id="app">
    <nav>
      <router-link to="/">Home Bagnan</router-link> |
      <router-link to="/about">INFORMATION</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #CE5937;
background: -moz-linear-gradient(left, #CE5937 0%, #1C6EA4 50%, #C59237 100%);
background: -webkit-linear-gradient(left, #CE5937 0%, #1C6EA4 50%, #C59237 100%);
background: linear-gradient(to right, #CE5937 0%, #1C6EA4 50%, #C59237 100%);
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
