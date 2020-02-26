<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
@import "@/components/global-styles/colors.scss";
// @import "./components/global-styles/colors.scss";
@import "@/components/global-styles/typography.scss";

#app {
  font-family: $system-font-family;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $white;
}
body {
  background-color: $dark-blue;
}
h1 {
  @include heading-1;
}
p {
  @include large-text-bold($purple);
}

#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: $white;
    }
  }
}
</style>
