<template>
  <nav>
    <!-- <router-link to="/">Home</router-link> -->
    <!-- We prefer this way of telling the link where to go, because we are good people -->
    <router-link :to="{name: 'home'}">Home</router-link>
  </nav>
  <router-view />
  <!-- 1. Create 2 new views: AboutView.vue & ContactView.vue in the "views" folder.
    In theese files, create a template tag at the top and inside you want a <div>, with a <h1> with the name of the viewfile
  -->

  <!-- 2. Update the router array (that is inside the @router/index.js) with the 2 new views -->

  <!-- 3. Update the App.vue with links to the new views (so thats with <router-link> and not <a href...>) -->

  <!-- 4. Lets start over:
        4.1 Add 2 new views: MissionView.vue & VisionView.vue
        4.2 Make it work so that theese new views are displayed in the nav and they work
  -->
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
